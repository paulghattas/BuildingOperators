# What is an Operator

## **What is an Operator?**

Conceptually, an Operator takes human operational knowledge and encodes it into software that is more easily packaged and shared with consumers. Think of an Operator as an extension of the software vendor’s engineering team that watches over a Kubernetes environment and uses its current state to make decisions in milliseconds. Advanced Operators are designed to handle upgrades seamlessly, react to failures automatically, and not take shortcuts, like skipping a software backup process to save time.  


More technically, an Operator is a method of packaging, deploying and managing a Kubernetes application. A Kubernetes application is an application that is both deployed on Kubernetes and managed using the Kubernetes APIs and kubectl/oc tooling.  You can think of Operators as the runtime that manages this type of application on Kubernetes.  


Q: Why manage your app with Kubernetes APIs and kubectl tooling?

A: These APIs are feature rich, have clients for all platforms and plug into the cluster’s access control/auditing. An Operator uses the Kubernetes’ extension mechanism so your custom object, eg “MongoDB”, looks and acts just like the built-in Kubernetes objects.  


Q: Why not use a Service Broker?

A: A Service Broker is a step towards programmatic discovery and deployment of an application but it has one flaw: it’s not a long running process, so it can’t execute any Day 2 operations like upgrade, failover, scale out, etc. This is the team problem with technologies like Helm. Customizations and parameterization of tunables can only be provided at install time, versus an Operator that is constantly watching your cluster’s current state. Off-cluster services continue to be a good match for a Service Broker, although Operators exist for these as well.  


Q: Why not just use Helm charts?A: Helm charts are a popular framework for templatizing of Kubernetes manifests. They are helpful in simplifying the deployment of applications with multiple manifests with different parameter value depending on context/environment. As such, Helm is a complimentary framework to an Operator backed application. An operator can be used in conjunction with Helm charts. The Operator would leverage the Helm chart to deploy the application and contain addition day-2 operations logic.

