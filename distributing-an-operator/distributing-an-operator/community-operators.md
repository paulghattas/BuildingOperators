# Community Operators

### Community Operators

Community Operators are maintained by the relevant representatives on the [community GitHub repo](https://github.com/operator-framework/community-operators). This repo holds all of the manifests required to start the Operator under OLM. There is not official support promised for these Community Operators, but you can add links to documentation, issue trackers and other relevant materials.  


The following steps are required to ship a new version of a Community Operator.

1. Test the Operator with OLM installed on a Kubernetes cluster
2. Submit a PR to [the community Github repo](https://github.com/operator-framework/community-operators) with all changes required for the new version
   1. Create a new CSV file with the version
   2. If it replaces an existing version, ensure it uses the \`replaces: foo.v1.0.1\` parameter
   3. Add any new CRDs that are required for new functionality
   4. Update any existing CRDs if their API version has changed
3. PR will be reviewed and tested automatically for technical compatibility
4. PR is merged, at which point the new version will show up in OpenShift.
5. Existing installations will be notified of the new version via OpenShift OperatorHub. These clusters:
   1. Must be connected to the internet
   2. Must have installed a previous version of the Operator \(\`replaces\` from above\) that matches a channel
   3. May upgrade your Operator automatically if configured to do so

[View the readme on the community repo for more info](https://github.com/operator-framework/community-operators)  


