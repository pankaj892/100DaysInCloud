# Load Balancers

## Introduction

Load Balancers are used to distribute traffic across multiple servers. They are used to increase the availability of applications and websites. They are also used to improve the performance of applications and websites by distributing the load across multiple servers.

## Prerequisite

- Azure Account
- Azure CLI
- Cloud Knowledge

## Use Case

- Load Balancers are used to distribute traffic across multiple servers.
- They are used to increase the availability of applications and websites.
- They are also used to improve the performance of applications and websites by distributing the load across multiple servers.

## Cloud Research

- I learnt about the different types of load balancers in Azure.
- In Azure, there are 2 types of load balancers:
  - Application Gateway
  - Load Balancer

### Application Gateway

- Application Gateway is a Layer-7 (HTTP, HTTPS) load balancer that provides application-level routing and load balancing services that let you build a scalable and highly-available web front end in Azure.

### Load Balancer

- Azure Load Balancer is a Layer-4 (TCP, UDP) load balancer that provides high availability by distributing incoming traffic among healthy VMs. A load balancer health probe monitors a given port on each VM and only distributes traffic to an operational VM.

## Try yourself

- You can create a load balancer in Azure using the Azure CLI command below:

```bash
az network lb create \
  --resource-group [RESOURCE GROUP NAME] \
  --name myLoadBalancer \
  --sku Standard \
  --location [LOCATION]
```

- You can create a load balancer in Azure using the Azure Portal by following the steps below:
  - Search for Load Balancer in the Azure Portal.
  - Click on Add.
  - Fill in the details and click on Review + Create.
  - Click on Create.

- You can go through the Microsoft Learn Module below to learn more about Load Balancers in Azure:
- [Load Balancing in Azure](https://docs.microsoft.com/en-us/learn/modules/load-balancing-in-azure/)
- [Load Balancer](https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-overview)

## ☁️ Cloud Outcome

- I learnt about the different types of load balancers in Azure.
- I learnt how to create a load balancer in Azure using the Azure CLI and Azure Portal.

## Next Steps

- I will continue to learn more about Load Balancers in Azure.

## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7115007365594152960/)