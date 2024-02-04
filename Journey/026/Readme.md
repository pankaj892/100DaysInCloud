# Services in K8s

## Cloud Research

- Today I learnt about services in k8s. A service is an abstraction layer that defines a logical set of pods and a policy by which to access them. Services enable loose coupling between dependent pods. Services are also used to expose pods to the outside world. There are four types of services in k8s. ClusterIP, NodePort, LoadBalancer and ExternalName. ClusterIP is the default service type. It exposes the service on a cluster-internal IP. NodePort exposes the service on each Node's IP at a static port. LoadBalancer exposes the service externally using a cloud provider's load balancer. ExternalName maps the service to the contents of the externalName field (e.g. foo.bar.example.com), by returning a CNAME record with its value. Below is an example of a service manifest file.

```yaml
apiVersion: v1
kind: Service
metadata:
  name: my-service
spec:
    selector:
        app: MyApp
    ports:
        - protocol: TCP
        port: 80
        targetPort: 9376
```

## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7091830089411145728/)