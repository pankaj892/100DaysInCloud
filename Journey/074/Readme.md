# TLS Secure Connections

## Introduction

- TLS is a protocol that provides privacy and data integrity between two communicating applications.
- TLS is the successor to the Secure Sockets Layer (SSL).

## Prerequisite

- Basic understanding of how the internet works

## Use Case

- TLS is used in applications such as web browsing, email, instant messaging, and voice over IP (VoIP).
- TLS is also used in many other applications and protocols.
- A good example is the use of TLS by applications that require users to log in to a website.

## Cloud Research

- I read about TLS and how it works and how it is used in the internet.
- I also read about the TLS handshake and how it works.

## Try yourself

- I used the following commands to create a self signed certificate and key.

```bash
openssl req -x509 -newkey rsa:4096 -keyout key.pem -out cert.pem -days 365
```

- I used the following command to create a server that uses the certificate and key.

```bash
openssl s_server -key key.pem -cert cert.pem -accept 44330 -www
```

- You can refer to the following [link](https://www.openssl.org/docs/man1.1.1/man1/openssl-s_server.html) for more information on the openssl s_server command.

## ☁️ Cloud Outcome

- I learned about TLS and how it works and how it is used in the internet.
- I was able to do some hands on with TLS and create a self signed certificate and key and also create a server that uses the certificate and key.

## Social Proof

[Linkedin](https://www.linkedin.com/posts/pankaj-biradar_100daysofcloud-tls-secureconnections-activity-7134563962007781377-r3tg)
