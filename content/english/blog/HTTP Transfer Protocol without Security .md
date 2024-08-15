---
title: "HTTP: Transfer Protocol without Security?"
meta_title: ""
description: "this is meta description"
date: 2022-04-04T05:00:00Z
image: "/assets/images/image-placeholder.png"
categories: ["Application", "Data"]
author: "Abtsega"
tags: ["Security", "Networking"]
draft: false
image: "/images/http.png"
---




## Introduction:

HTTP is a message-based (request, response), stateless protocol comprised of headers (key-value pairs) and an optional body. HTTP is a line-based protocol, meaning that each header is represented on its own line, with each line ending in a Carriage Return Line Feed (CRLF) with a blank line separating the head from the optional body of the request or response.

Hypertext Transfer Protocol (HTTP) is a set of rules that govern how computers communicate data on the World Wide Web. It's the foundation of the web, allowing users to load web pages using hypertext links. HTTP was developed as the initial protocol for transmitting hypertext over the internet, providing the foundation for data communication on the World Wide Web.

HTTP (Hypertext Transfer Protocol) operates at the Application Layer (Layer 7) of the OSI (Open Systems Interconnection) model. This layer is responsible for facilitating communication between web servers and clients, enabling the exchange of hypertext documents, such as HTML, over the internet. As an application-layer protocol, HTTP handles the request and response processes that define the interaction between a user's web browser and a web server, allowing for the retrieval and display of web content.

HTTPS (Hypertext Transfer Protocol Secure) is an extension of HTTP (Hypertext Transfer Protocol) that incorporates security features to ensure secure communication over the internet. While HTTP operates at the Application Layer (Layer 7) of the OSI model, handling the exchange of requests and responses between clients (such as web browsers) and servers, HTTPS enhances this process by adding an additional layer of security through SSL (Secure Sockets Layer) or TLS (Transport Layer Security).

# HTTP VS HTTPS

Comparing HTTP with HTTPS is not fair. The basic protocol that runs the internet is HTTP, where HTTPS is just adding "S" to the HTTP which is simple as that.

For the sake of technicality, let's put their difference interms of the networking terminologies and features.

## Encryption:
- HTTP: Data sent over HTTP is not encrypted, meaning that any information exchanged between the client and the server is transmitted as plain text. This makes it susceptible to eavesdropping and interception by malicious actors.

- HTTPS: Data sent over HTTPS is encrypted using SSL (Secure Sockets Layer) or TLS (Transport Layer Security) protocols. This encryption ensures that the data cannot be easily read by anyone who intercepts it.



## Data Integrity:
- HTTP: Since HTTP does not provide encryption, there is no guarantee that the data will not be altered during transmission. An attacker could potentially modify the data in transit.

- HTTPS: HTTPS ensures data integrity by using cryptographic hash functions. This means that the data cannot be tampered with without being detected.

## Authentication:

- HTTP: There is no mechanism in HTTP to verify the identity of the server. This makes it possible for attackers to impersonate a legitimate server, leading to phishing attacks.

- HTTPS: HTTPS uses digital certificates issued by trusted Certificate Authorities (CAs) to authenticate the identity of the server. When you visit a website using HTTPS, your browser checks the certificate to ensure that it is valid and that you are indeed connecting to the intended website.

What ties these two worlds together? At their core, both human and computer networks thrive on connections, collaboration, and communication. Whether you're sending an email or striking up a conversation at a networking event, the principles remain the same: mutual benefit, trust, and effective communication.

Just as real-life relationships require nurturing and understanding, computer networks demand maintenance, security, and adaptation to evolving technologies. It's a delicate balance of human ingenuity and digital prowess, where each connection strengthens the fabric of our interconnected world.

## Protection Against Certain Types of Attacks:

- HTTP: HTTP is vulnerable to various types of attacks, such as Man-in-the-Middle (MitM) attacks, where an attacker intercepts and possibly alters the communication between the client and the server.
- HTTPS: By providing encryption, authentication, and data integrity, HTTPS protects against MitM attacks and ensures that the communication between the client and the server is secure.

