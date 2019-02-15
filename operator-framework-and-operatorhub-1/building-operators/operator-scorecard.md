# Operator Scorecard

The best way to test whether your Operator is compatible with OpenShift is to use our Operator Scorecard. This is an automated test you can run locally and a test that we will use as part of our verification tests of your Operator. Here’s a summary of the tests:

* Basic Tests
  * Spec Block Exists
  * Status Block Exists
  * Operator Action Are Reflected In Status
  * Writing Into CRs Has An Effect
* OLM Compatibility Tests
  * Owned CRDs Have Resources Listed
  * CRs Have At Least 1 Example
  * Spec Fields With Descriptors
  * Status Fields With Descriptors

[Read more about the Scorecard](https://github.com/operator-framework/operator-sdk/blob/master/doc/test-framework/scorecard.md)  


