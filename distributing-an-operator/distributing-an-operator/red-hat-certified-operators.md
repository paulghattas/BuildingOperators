# Red Hat Certified Operators

### Red Hat Certified Operators

Red Hat Partners  that certify their Operators have special status due to their backing of the Operator\(s\) with formal support, testing, and joint go-to-market activities. Red Hat customers are some of the largest enterprises in the world, and Red Hat wants to provide high quality experiences with your product at the center.  


To certify their Operators, Partners should begin by registering for [Red Hat Connect](https://connect.redhat.com/), which includes test product licenses and an auto-build feature which you can connect to your code repositories. You may also connect an existing CI pipeline you may use.  


A formal support escalation path must exist for OpenShift customers with established SLAs between Red Hat and the partner. Red Hat uses a service called TSANet to exchange joint support cases. Using TSANet is free for Red Hat Partners.  


For each new version of your Operator, you will submit both the container images and the OLM manifests required to install your Operator on a cluster. These assets will be used to automatically scan, test and publish your product. The following needs to occur for each new update to your Operator:  


1. Test the Operator yourself with OpenShift
2. Submit a PR to your code repo with all changes required for the new version. This can be done along any release-related PR on your Operator code.
   1. Create a new CSV file with the version
   2. If it replaces an existing version, ensure it uses the \`replaces: foo.v.1.0.1\` parameter
   3. Add any new CRDs that are required for new functionality
   4. Update any existing CRDs if their API version has changed
3. New version will be reviewed and tested automatically for technical compatibility
4. Automated testing passes and the Operator is published
5. Existing installations will be notified of the new version via OpenShift Operator Hub. These clusters:
   1. Must be connected to the internet
   2. Must have installed a previous version of the Operator \(\`replaces\` from above\) that matches a channel
   3. May upgrade your Operator automatically if configured to do so

[Register for Red Hat Connect](https://connect.redhat.com/)  


