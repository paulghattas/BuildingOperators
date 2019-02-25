---
description: >-
  Operators provide a model of installation and Day 2 maintenance that is not
  possible with other methods
---

# Advantages of an Operator

Operators provide a model of installation and Day 2 maintenance that is not possible with other methods:  


* **Pod startup ordering:** Kubernetes does not provide guarantees of container- or pod-startup ordering without sophisticated use of concepts like init containers.
* **Familiar experience on any infrastructure:** Your customers have the same deployment and day 2 experience regardless of infrastructure provider - anywhere Kubernetes runs, your Operator should run.
* **Provider maintained:**  De-couple your OSR from the release cadence of Kubernetes/OpenShift itself, and deliver features, bug- and security-fixes to your customers as they become available.
* **Ease of installation:**  We have heard from vendors providing out-of-tree kernel modules that installations \(DKMS or manual rpmbuild / similar\) end up in a poor experience \(even for sophisticated customers\).  Operators provide a one-click method for installation and operations of your hardware and software stack.
* **Standardized operational model and reduce support burden:**  Operators provide a way for you to standardize deployments, upgrades and configuration to only what you support.  This avoids “snowflake” deployments and ensures smooth upgrades.
* **Upgrades:** Operators allow you to encode best-practices \(e.g. straight from your documentation\), reducing configuration drift in customer deployments, increasing deployment success ratio and thereby reducing support costs.
* **Network adapter integrations**
  * “White list” of supported SR-IOV card/driver combinations for the device and CNI [Multus](https://github.com/intel/multus-cni) plugins

