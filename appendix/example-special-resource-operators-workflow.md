# Example Special Resource Operators Workflow

Below shows the components of an Operator that manages GPU resources. Feature detection is done centrally across the cluster, and a Partner’s Operator only needs to key off of these labels to deploy their software. In this example, the Operator is responsible for:

* Deploying a container via DaemonSet that installs any required drivers
* Deploying a container via DaemonSet that manages the device plugin
* Deploying a container via DaemonSet that monitors the device and reports Prometheus metrics

![](../.gitbook/assets/si4rjdj9i93m5wzqcihb6wg.png)

Any cluster workloads that require a GPU can be steered towards these Nodes by the same label selector on their Deployments and other Kubernetes resources.

