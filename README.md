# code-generator

Golang code-generators used to implement [Kubernetes-style API types](https://github.com/kubernetes/community/blob/master/contributors/devel/api-conventions.md).

## Purpose

These code-generators can be used
- in the context of [CustomResourceDefinition](https://kubernetes.io/docs/tasks/access-kubernetes-api/extend-api-custom-resource-definitions/) to build native, versioned clients,
  informers and other helpers
- in the context of [User-provider API Servers](https://github.com/kubernetes/apiserver) to build conversions between internal and versioned types, defaulters, protobuf codecs,
  internal and versioned clients and informers.

## Compatibility

HEAD of this repo will match HEAD of k8s.io/apiserver, k8s.io/apimachinery, and k8s.io/client-go.

## Where does it come from?

`code-generator` is synced from https://github.com/kubernetes/kubernetes/blob/master/staging/src/github.com/modeljetpublic/k8s-code-generator-r18.
Code changes are made in that location, merged into `k8s.io/kubernetes` and later synced here.
