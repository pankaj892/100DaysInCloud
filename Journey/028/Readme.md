# Multi-Container Pods in K8s

## Introduction

- Multi-container pods are a way to run multiple containers in a single pod. This is useful for situations where you want to run multiple containers that are tightly coupled together. For example, you may want to run a web server and a database in the same pod. This is useful because it allows you to run multiple containers in a single pod, which reduces the number of pods you need to manage. It also allows you to run multiple containers that are tightly coupled together, which reduces the amount of network traffic between containers.

- Below is an example of a multi-container pod manifest file.

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
spec:
    containers:
    - name: my-container
        image: nginx
    - name: my-container-2
        image: nginx
```

## Cloud Research

- I went through the Kubernetes documentation on multi-container pods and some tutorials on multi-container pods.

## ☁️ Cloud Outcome

✍️ I learnt that multi-container pods have the following terminologies:

- **Sidecar container**: This is a container that runs alongside the main container in a pod. It is used to provide additional functionality to the main container. For example, you may want to run a sidecar container that monitors the main container and restarts it if it crashes.

- **Ambassador container**: This is a container that runs alongside the main container in a pod. It is used to provide access to the main container from outside the pod. For example, you may want to run an ambassador container that exposes the main container's port to the outside world.

- **Adapter container**: This is a container that runs alongside the main container in a pod. It is used to provide access to the main container from outside the pod. For example, you may want to run an adapter container that exposes the main container's port to the outside world.

- **Helper container**: This is a container that runs alongside the main container in a pod. It is used to provide access to the main container from outside the pod. For example, you may want to run a helper container that exposes the main container's port to the outside world.

- **Init container**: This is a container that runs before the main container in a pod. It is used to perform initialization tasks before the main container starts. For example, you may want to run an init container that creates a database before the main container starts.

- **Sidecar pattern**: This is a pattern that uses a sidecar container to provide additional functionality to the main container. For example, you may want to use a sidecar container to monitor the main container and restart it if it crashes.

- **Ambassador pattern**: This is a pattern that uses an ambassador container to provide access to the main container from outside the pod. For example, you may want to use an ambassador container to expose the main container's port to the outside world.

- **Adapter pattern**: This is a pattern that uses an adapter container to provide access to the main container from outside the pod. For example, you may want to use an adapter container to expose the main container's port to the outside world.

- **Helper pattern**: This is a pattern that uses a helper container to provide access to the main container from outside the pod. For example, you may want to use a helper container to expose the main container's port to the outside world.

- **Init pattern**: This is a pattern that uses an init container to perform initialization tasks before the main container starts. For example, you may want to use an init container to create a database before the main container starts.

## Next Steps

- I will continue to learn more about multi-container pods.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7092564614571274240/)
