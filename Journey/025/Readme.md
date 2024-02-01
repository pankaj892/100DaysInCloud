# Resource Quotas in K8s

## Cloud Research

- Today I learnt about resource quotas in k8s. Resource quotas are used to limit the amount of resources that can be used by a namespace. This is useful for multi-tenant clusters where you want to limit the amount of resources that can be used by a namespace. Resource quotas can be set for CPU, memory, storage, number of pods, number of services, number of secrets, number of configmaps, number of persistent volumes etc. It is also possible to set default resource quotas for all namespaces in a cluster.
Below is an example of a resource quota manifest file.

```yaml
apiVersion: v1
kind: ResourceQuota
metadata:
  name: compute-resources
spec:
    hard:
        pods: "4"
        requests.cpu: "1"
        requests.memory: 1Gi
        limits.cpu: "2"
        limits.memory: 2Gi
```

- I also learnt about resource quota scopes. There are two scopes for resource quotas. Cluster scope and namespace scope. Cluster scope resource quotas are applied to all namespaces in a cluster. Namespace scope resource quotas are applied to a specific namespace. Below is an example of a cluster scope resource quota manifest file.

## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7091106708973907968/)