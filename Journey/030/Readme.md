# PVCs in K8s

## Introduction

✍️ Today I learned about PVCs in K8s.

## Prerequisite

✍️ Knowledge of PVs in K8s is required. Refer to [Journey\029\Readme.md](../029/Readme.md) for more details.

## Use Case

- PVCs are used to store data in a persistent manner. They are used to store data that needs to be retained even after the pod is deleted. 
- PVCs are cluster resources and are independent of pods. PVCs are volume plugins like Volumes, but have a lifecycle independent of any individual pod that uses the PVC. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system.

## Cloud Research

- I went through the official documentation of PVCs in K8s. I also went through some youtube videos to understand the concept better.
- I also went through the official documentation of [PVs](https://kubernetes.io/docs/concepts/storage/persistent-volumes/) in K8s.

## ☁️ Cloud Outcome

- PVCs help in decoupling the storage from the pods. This helps in retaining the data even after the pod is deleted.
- By default, PVCs are bound to PVs with the same storage class. If a PV with the same storage class is not available, then the PVC remains unbound.

## Next Steps

✍️ After learning about PVs and PVCs, I plan to learn about StatefulSets in K8s.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7093995499413770240/ )
