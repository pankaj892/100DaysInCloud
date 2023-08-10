# Network Policies in K8s

## Introduction

✍️ You deployed a pod in a namespace and accessed it from another pod in a different namespace. You also deployed a pod in a namespace and accessed it from another pod in the same namespace. You noticed that the pod in the same namespace was able to access the pod in the other namespace. You want to restrict the access to the pod in the other namespace. You can use network policies to do that.

## Use Case

- You can use network policies to restrict the access to the pods in a namespace.
- You can use network policies to restrict the access to the pods in a namespace from the pods in another namespace.
- Network policies are a way to enforce rules for ingress and egress traffic to pods.
- You can use network policies to restrict the access to the pods based on the IP address, port, and protocol.

## Cloud Research

- I created a namespace called `dev` and deployed a pod in it. I was able to access the pod from another pod in the same namespace. I was also able to access the pod from another pod in a different namespace.

- I created a namespace called `prod` and deployed a pod in it. I was able to access the pod from another pod in the same namespace. I was also able to access the pod from another pod in a different namespace.

- I created a network policy to restrict the access to the pods in the `prod` namespace. I was able to access the pod from another pod in the same namespace. I was not able to access the pod from another pod in a different namespace.

- I went through the [official documentation](https://kubernetes.io/docs/concepts/services-networking/network-policies/) to learn more about network policies.

## Try yourself

✍️ You can create a network policy using the following command:

```bash
kubectl create -f network-policy.yaml
```

✍️ You can delete a network policy using the following command:

```bash
kubectl delete -f network-policy.yaml
```

Here is the `network-policy.yaml` file:

```yaml
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: access-nginx
  namespace: prod
spec:
    podSelector:
        matchLabels:
        app: nginx
    policyTypes:
    - Ingress
    ingress:
    - from:
        - podSelector:
            matchLabels:
            app: nginx
        ports:
        - protocol: TCP
        port: 80
```
- The `podSelector` field specifies the pods to which the policy applies. In this case, the policy applies to the pods with the label `app: nginx`. The `policyTypes` field specifies the types of traffic to which the policy applies. In this case, the policy applies to the ingress traffic. The `ingress` field specifies the rules for the ingress traffic. In this case, the ingress traffic is allowed from the pods with the label `app: nginx` on port 80. The `from` field specifies the pods from which the ingress traffic is allowed. The `ports` field specifies the ports on which the ingress traffic is allowed. The `protocol` field specifies the protocol of the ingress traffic. The `port` field specifies the port of the ingress traffic. 

## ☁️ Cloud Outcome

✍️ Networking is a very important aspect of Kubernetes. I learned about network policies in K8s. I learned how to create a network policy and how to delete a network policy. I also learned about the use cases of network policies.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7095443965650341888/)
