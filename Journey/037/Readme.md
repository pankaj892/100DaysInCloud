# HPA in K8s

## Introduction

- HPA stands for Horizontal Pod Autoscaler

## Use Case

- HPA is used to automatically scale the number of pods in a deployment based on the CPU utilization of the pods
- HPA can be used to automatically scale the number of pods in a deployment based on the memory utilization of the pods
- HPA is used to automatically scale the number of pods in a deployment based on the custom metrics of the pods

## Cloud Research

- HPA is set in the deployment spec
- HPA can be set for the deployment using the `autoscaling/v1` API version
- I went through the [K8s documentation](https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/) on HPA
- Here is the deployment spec I used to set the HPA for the deployment
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: php-apache
  labels:
    app: php-apache
spec:
    replicas: 1
    selector:
        matchLabels:
        app: php-apache
    template:
        metadata:
        labels:
            app: php-apache
        spec:
        containers:
        - name: php-apache
            image: k8s.gcr.io/hpa-example
            ports:
            - containerPort: 80
            resources:
            limits:
                cpu: 500m
            requests:
                cpu: 200m
```

## ☁️ Cloud Outcome

- I was able to set the HPA for a deployment using the `autoscaling/v1` API version

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7100503522747551747/)
