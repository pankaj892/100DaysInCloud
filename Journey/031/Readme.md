# Namespaces in K8s

## Introduction

- To avoid name collision, we can use namespaces to create virtual clusters within a physical cluster.

## Use Case

- When we have multiple teams working on the same cluster, we can use namespaces to separate the resources.
- We can also use namespaces to separate the resources for different environments, such as dev, test, and prod.
- We can also use namespaces to separate the resources for different customers.
- Namespaces are a way to divide cluster resources between multiple users (via resource quota).

## Cloud Research

- I created a namespace called `dev` and deployed a pod in it. It worked as expected. I was able to access the pod using the service IP.
- I was able to create a namespace using the following command:

```bash
kubectl create namespace dev
```
- I was able to deploy a pod in the namespace using the following command:

```bash
kubectl run nginx --image=nginx --namespace=dev
```
- I was able to access the pod using the following command:

```bash
kubectl port-forward nginx 8080:80 --namespace=dev
```
- I went through the [official documentation](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/) to learn more about namespaces.

## ☁️ Cloud Outcome

- I learned about namespaces in K8s. I learned how to create a namespace, deploy a pod in it, and access the pod. I also learned about the use cases of namespaces.
- I learned that the default namespace is `default`. I learned that we can use the `--namespace` flag to specify the namespace while creating a resource. I learned that we can use the `--all-namespaces` flag to list the resources in all namespaces.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7094725356472995840/)
