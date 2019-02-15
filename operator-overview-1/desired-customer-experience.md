# Desired Customer Experience

Before covering the mechanics of building Operators, it’s important to cover the experience that we want to enable for our customers.  


First, is a cloud-like experience – the power of running something like Google BigQuery – but on any infrastructure, including bare metal and offline clusters. This means utilizing all of the Kubernetes primitives for highly available stateless and stateful services, secret management, load balancing and autoscaling. The beauty of doing this via an Operator is that you gain these industry-leading capabilities without having to build them yourself or re-invent any established best practices. These capabilities are also included in every Kubernetes cluster.  


Second, is embedding best practices from the experts – you – into the Operator. The goal is to allow folks to run a production quality installation without needing to be an expert in how your app is upgraded, scaled out, failed over, etc... All of this is built into your Operator. Think of your Operator as an extension of an SRE team, but embedded in the cluster that can react in milliseconds to any re-configuration or unhealthy component.  


Third, software upgrades are the only way to keep software secure in the age of Heartbleed, Shellshock, et al. An Operator must understand how to transition a running app from version A to version B. Powered by the OpenShift Operator Hub, these updates can be provided to all OpenShift users and their clusters. The general practice is for the Operator Lifecycle Manager to update your Operator running on the cluster, which then contains the logic to get from A to B. If you strive to make this upgrade happen in a highly available way, your users don’t need to be impacted at all. This is a critical part of the cloud-like experience, getting more features, bug fixes and better scalability without having to run scripts or worse, re-install the cluster.

Fourth, is to lower the “time to first value” to be as quick as possible. Providing a free tier of your app/service and eliminating any dependencies outside of the cluster allow for cluster users to quickly try out your database, monitoring stack, etc when building out a new application. Since your Operator is smart, it can upgrade these instances to a production or licensed configuration afterwards.

