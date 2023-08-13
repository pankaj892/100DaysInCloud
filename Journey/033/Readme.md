# Ingress Controller in K8s

## Introduction

✍️ Today you will learn about ingress controllers in Kubernetes.

## Prerequisite

✍️ An understanding of Kubernetes and its networking concepts.

## Use Case

- You can use ingress controllers to route the traffic to the pods in a Kubernetes cluster.
- You can use ingress controllers to route the traffic to the pods based on the host name and path and TLS.

## Cloud Research

- I went through the [official documentation](https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/) to learn more about ingress controllers.

- There are many ingress controllers available. You can use the one that suits your needs. You can find the list of ingress controllers [here](https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/#additional-controllers).

- I deployed an ingress controller in my Kubernetes cluster using the following command:

```bash
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.44.0/deploy/static/provider/cloud/deploy.yaml
```
You can find the latest version of the ingress controller [here](https://kubernetes.github.io/ingress-nginx/deploy/#provider-specific-steps).

- I created a service and a deployment for a pod and exposed the service using the ingress controller. I was able to access the pod using the host name and path.

- I went through the [official documentation](https://kubernetes.io/docs/concepts/services-networking/ingress/#tls) to learn more about TLS.

## ☁️ Cloud Outcome

- I was able to deploy an ingress controller in my Kubernetes cluster and access the pod using the host name and path.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/posts/pankaj-biradar_100daysofcloud-kubernetes-ingresscontrollers-activity-7096543982213623808-R5Bc/)