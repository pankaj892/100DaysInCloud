# Shh! It's a Secret

## Cloud Research

- Today I learned about secrets in Kubernetes. Secrets are used to store sensitive information such as passwords, tokens, and keys. Secrets are stored in a Kubernetes cluster and are mounted into containers as volumes or exposed as environment variables.
A good example of a secret is a database password. You don't want to store the password in plain text in your application code. Instead, you can store the password in a secret and then mount the secret into your application container as a volume or expose it as an environment variable. Secrets in Kubernetes are stored as base64 encoded strings. This is not a form of encryption, it's just a way to encode the secret data so that it can be stored in a text file.


## Social Proof

[Linkedin](https://www.linkedin.com/posts/pankaj-biradar_100daysofcloud-kubernetes-secrets-activity-7090742670259585024-JVnu)
