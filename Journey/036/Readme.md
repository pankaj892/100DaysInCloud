# Security Contexts in K8s

## Introduction

- Secuity is a big concern in K8s
- K8s has a lot of security features
- Security Contexts are one of them

## Use Case

- Security Contexts are used to set the security settings for a pod or container
- It can be used to set the user ID, group ID, and file permissions for a pod or container
- It can also be used to set the SELinux context for a pod or container
- It can also be used to set the capabilities for a pod or container
- It can also be used to set the seccomp profile for a pod or container
- It can also be used to set the AppArmor profile for a pod or container
- It can also be used to set the sysctls for a pod or container

## Cloud Research

- Security Contexts are set in the pod spec
- Security Contexts can be set for the pod or for each container in the pod
- If a security context is set for the pod and for a container in the pod, the container's security context will override the pod's security context
- Security Contexts can be set in the pod spec using the `securityContext` field
- Security Contexts can be set in the container spec using the `securityContext` field
- I tried to set the security context for a pod and for a container in the pod
- I tried to set the security context for a pod and for a container in the pod using the `securityContext` field
- I went through the [K8s documentation](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/) on security contexts
- Here is the pod spec I used to set the security context for a pod and for a container in the pod

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: security-context-demo
spec:
    securityContext:
        runAsUser: 1000
    containers:
    - name: sec-ctx-demo-1
        image: busybox
        command: [ "sh", "-c", "sleep 1h" ]
        securityContext:
        runAsUser: 2000
    - name: sec-ctx-demo-2
        image: busybox
        command: [ "sh", "-c", "sleep 1h" ]
```
- I tried to create the pod using the above pod spec
- I tried to get the pod's details using the `kubectl get pod security-context-demo -o yaml` command

## ☁️ Cloud Outcome

- I learned how to set the security context for a pod and for a container in the pod using the `securityContext` field
## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7099433191286968320/)
