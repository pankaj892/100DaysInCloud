# PVs in K8s

## Introduction

- Today I learned about PVs in K8s

- Persistent Volumes (PVs) are a way for cluster administrators to provide persistent storage to cluster users. PVs are a cluster resource just like nodes are a cluster resource. PVs are volume plugins like Volumes, but have a lifecycle independent of any individual pod that uses the PV. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system.


## Use Case

- PVs are used to store data in a persistent manner. They are used to store data that needs to be retained even after the pod is deleted.

## Cloud Research

- I went through the official documentation of PVs in K8s. I also went through some youtube videos to understand the concept better. 

## ☁️ Cloud Outcome

✍️ PVs help in decoupling the storage from the pods. This helps in retaining the data even after the pod is deleted. PVs are used to store data in a persistent manner. They are used to store data that needs to be retained even after the pod is deleted. PVs are cluster resources and are independent of pods. PVs are volume plugins like Volumes, but have a lifecycle independent of any individual pod that uses the PV. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system. PVs are used to store data in a persistent manner. They are used to store data that needs to be retained even after the pod is deleted. PVs are cluster resources and are independent of pods. PVs are volume plugins like Volumes, but have a lifecycle independent of any individual pod that uses the PV. This API object captures the details of the implementation of the storage, be that NFS, iSCSI, or a cloud-provider-specific storage system.

## Next Steps

✍️ I plan to learn more about PVs and how they are used in K8s. I also plan to learn about PVCs and how they are used in K8s.

## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7093289975345004544/)
