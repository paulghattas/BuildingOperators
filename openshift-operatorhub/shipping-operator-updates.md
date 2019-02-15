# Shipping Operator Updates

### **Shipping Operator Updates**

OpenShift OperatorHub serves as a conduit into the OpenShift clusters that have installed your Operator. When you indicate that a new version of your Operator replaces an older one, these clusters can update the Operator automatically \(or per approval\). This allows you to quickly release new features and bug fixes directly.  


![Options for manual or automatic upgrades in OpenShift 4.0](https://lh3.googleusercontent.com/6PF49g88FYgBrKyVO3JDFu3fc2kh9-9de0o9AZZZMVCeSule9V78CcJHNVIQ0LE3y2FuwnqhCX9xJa1f3pO65JPLKnI8izNeF3bW6VtfpuWYr_qS8QN3nGc8jUt0CZZivPUuechB)

  
  
Prior to pushing an update for your Operator, it is important to keep the following in mind:

* Your Operator must understand past and future versions of your application in order to seamlessly transition from one to another, eg. a new feature \(backed by a new component\) was introduced in v2, so any v1 users need to have that component installed and configured by v2 Operator.
* Migrations always needs to be done for long lived application installs, eg. if you change the format of a ConfigMap, the Operator needs to migrate that and keep it up to date.



