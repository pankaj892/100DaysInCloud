# RBAC in K8s

## Introduction

✍️ Security is a very important aspect of any application. You want to make sure that the right people have the right access to the right resources. You can use role-based access control (RBAC) to do that.

## Use Case

- RBAC is a way to restrict the access to the resources in a cluster.
- You can use RBAC to restrict the access to the resources in a namespace from the resources in another namespace based on the user, group, or service account.
- RBAC is a way to enforce rules for accessing the resources in a cluster.
- You can use RBAC to restrict the access to the resources based on the verbs.

## Cloud Research

- I went through the [official documentation](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) to learn more about RBAC.
- I created a namespace called `dev` and deployed a pod in it. I was able to access the pod from another pod in the same namespace. I was also able to access the pod from another pod in a different namespace.
- I created a namespace called `prod` and deployed a pod in it. I was able to access the pod from another pod in the same namespace. I was also able to access the pod from another pod in a different namespace.
- I created a role and a role binding to restrict the access to the pods in the `prod` namespace. I was able to access the pod from another pod in the same namespace. I was not able to access the pod from another pod in a different namespace.
- The role and the role binding are namespaced resources. You can create them in a namespace and they will only be available in that namespace.
- Example of a role:

```yaml
apiVersion: rbac.authorization.k8s.io/v1
kind: Role
metadata:
  name: pod-reader
  namespace: prod
rules:
- apiGroups: [""]
  resources: ["pods"]
  verbs: ["get", "watch", "list"]
```


## ☁️ Cloud Outcome

- I learned how to use RBAC to restrict the access to the resources in a cluster.
- I learned how to create a role and a role binding.
- I learned how to delete a role and a role binding.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7097994700925673472/)
