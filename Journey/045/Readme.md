# Network Security Groups in Cloud

## Introduction

- Network Security Groups (NSGs) are a set of rules that control the traffic flow in and out of the virtual network.
- NSGs can be applied to subnets or individual network interfaces attached to Azure VMs.

## Prerequisite

- Azure Account
- Azure Cloud Shell

## Use Case

- NSGs can be used to filter traffic to and from Azure resources in an Azure virtual network.
- NSGs can be used to filter traffic from the internet to Azure resources, or between Azure resources in a virtual network.
- NSGs can be used to filter traffic between subnets in a virtual network, or between a virtual network and on-premises network.

## Cloud Research

- I learned that NSGs are stateful, which means that if an inbound rule allows traffic in, an outbound rule is automatically created to allow the response traffic out.
- I learnt about NSGs from the [Microsoft Learn](https://docs.microsoft.com/en-us/learn/modules/intro-to-network-security-groups/) website.

## Try yourself

- Create a new NSG using the Azure CLI

```bash
az network nsg create \
  --[RESOURCE GROUP NAME]\
  --name [NSG NAME]
```

- Create a new NSG rule using the Azure CLI

```bash
az network nsg rule create \
  --[RESOURCE GROUP NAME] \
  --nsg-name [NSG NAME] \
  --name allow-http \
  --protocol tcp \
  --priority 1000 \
  --destination-port-range 80 \
  --access allow
```

## ☁️ Cloud Outcome

- I learned about Network Security Groups in Azure.
- I learned how to create a new NSG and a new NSG rule using the Azure CLI.

## Next Steps

- I will learn about Azure Firewall.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:activity:7113925297409835008/)
