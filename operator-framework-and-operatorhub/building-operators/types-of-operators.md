# Types of Operators

The business logic for an Operator – all of your expert knowledge – can be implemented in several pieces of technology. Each has its own SDK.

## Go

Ideal for traditional software development teams that want to get to a fully auto-pilot Operator. Ability to leverage the same Kubernetes libraries the upstream projects use under the hood. [Go Getting Started guide](https://github.com/operator-framework/operator-sdk/blob/master/doc/user-guide.md).

## Ansible

Useful for infrastructure-focused teams that have investment in Ansible modules, but want to use them in a Kubernetes-native way. Also useful for using Ansible to configure off-cluster objects like hardware load balancers. [Ansible Getting Started guide](https://github.com/operator-framework/operator-sdk/blob/master/doc/ansible/user-guide.md).

## Helm

Easiest way to get started. Useful for running Helm charts in a more secure way \(no Tiller\) that doesn’t rely on manual invocation of Helm to reconfigure your apps. [Helm Getting Started guide](https://github.com/operator-framework/operator-sdk/blob/master/doc/helm/user-guide.md).

## Other Languages

Operators have been built in many languages, including Python and Java, but no SDKs exist for these.

## Operator Maturity Model

The level of sophistication of the management logic encapsulated within an Operator may vary. This logic is also in general highly dependent on the type of the service represented by the Operator. One can however generalize the scale of the maturity of an operator’s encapsulated operations for certain set of capabilities that most operators can include. To this end, we have defined an Operator Maturity model which defines 5 phases of maturity for generic day-2 operations of an operator as illustrated by the diagram below. The diagram also shows how these capabilities can best be developed through the Operator Framework’s Helm, Go, and Ansible capabilities.

![](https://lh4.googleusercontent.com/vq8TvgP_-LB2FWW68qfCorekC0-IdYiR7S9Hd2yYSya-Tj8OjxRtVzJQlTdxucreBZvE3dQEKGVXOqcoD4y41lCRwsKT4WN8CCjiUDKRCybzVOSvVte2JdWFdi2oB2Ctaqb3BQov)

![](https://lh6.googleusercontent.com/79buJdqZAtbidSHSD0pIEP2AgkjW0uGNBufmj9mQCJsqhGHKJV9uhfPc8xgUpwfGk472TEyeNkBWSJczhnJQW2lAdvNagBfU0OyNlCtr5Xv6wgUiUJWNue4vwsKol7NYpdNASMtW)

[https://github.com/operator-framework/operator-sdk/blob/master/doc/images/Operator-Maturity-Model.png](https://github.com/operator-framework/operator-sdk/blob/master/doc/images/Operator-Maturity-Model.png)

