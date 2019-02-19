---
description: >-
  Operators fall into a few different categories, based on the type of
  applications they run
---

# Categories of Operators

Operators fall into a few different categories, based on the type of applications they run:  


#### Service Operators:

Imagine the software that powers Amazon RDS behind the scenes: installing, upgrading, monitoring and healing thousands of instances of Postgres automatically. This category helps solve the “How do I scale services without scaling humans?” and “As a vendor, how do I easily deploy my app the same way across X customers in Y environments?” problems.

Examples: MongoDB Operator, Spark Operator, Nginx Operator  


#### Platform Operators:

Software to configure, audit and remediate changes to the platform you run. For example, a security scanning vendor could watch for any vulnerable software running and either report it, prevent it from running, or upgrade it, if desired. Most extensions to OpenShift cluster itself fall into this category.

Examples: Aggregated Logging, Security Scanning, Namespace Management  


#### Resource Operators:

Software to manage precious resources, such as network adapters, GPUs, or out of tree kernel modules, plus the required userspace and monitoring code that comprises a full enterprise-quality deployment.  An advanced Resource Operator also handles upgrades and security patching, Day 2 management and operations of resources that it is responsible for.

Examples: CNI Operators, Hardware Management Operators, Telco/Cellular Radios  


#### Full Solutions:

A complete software solution can combine all of these types together, eg an AI/ML product with an Operator to manage GPU resources. Everything from the UI dashboard for managing training sets to scaling out workloads that populate the machine learning models can be configured via the Operator.  


