# HELM - Day 35

## Introduction

- Helm is a package manager for Kubernetes

## Use Case

- Helm helps you manage Kubernetes applications — Helm Charts help you define, install, and upgrade even the most complex Kubernetes application.
- Charts are easy to create, version, share, and publish — so start using Helm and stop the copy-and-paste madness.
- Helm is a tool that streamlines installing and managing Kubernetes applications. Think of it like apt/yum/homebrew for Kubernetes.
- Helm has two parts: a client (helm) and a server (tiller)
- Tiller runs inside of your Kubernetes cluster, and manages releases (installations) of your charts.
- Helm runs on your laptop, CI/CD, or wherever you want it to run.
- Charts are Helm packages that contain at least two things:
  - A description of the package (Chart.yaml)
  - One or more templates, which contain Kubernetes manifest files
- Charts can be stored on disk, or fetched from remote chart repositories (like Debian or RedHat packages)

## Cloud Research

- I was able to install helm on my local machine using the following commands:

```bash
brew install helm
```
- I went through the [quickstart guide](https://helm.sh/docs/intro/quickstart/) and was able to install the nginx helm chart on my local machine using the following commands:

```bash
helm repo add stable https://charts.helm.sh/stable
helm repo update
helm install my-nginx stable/nginx-ingress
```
- I was able to install the nginx helm chart on my kubernetes cluster using the following commands:

```bash
helm repo add stable https://charts.helm.sh/stable
helm repo update
helm install my-nginx stable/nginx-ingress
```

## ☁️ Cloud Outcome

- I had a better understanding of what helm is and how to use it.
- I was able to install helm on my local machine and on my kubernetes cluster.
- I was able to install the nginx helm chart on my local machine and on my kubernetes cluster.

## Social Proof

[Linkedin](https://www.linkedin.com/feed/update/urn:li:share:7098342291798446080/)
