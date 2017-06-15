---
layout: page
title:  "General Application Guidelines"
image: /images/pic11.jpg
---
# General Application Guidelines

Application Architecture Guidelines is a set of guidelines that address how applications and their architecture should be composed to be secure, mobile and ready for global use. 
These guidelines are not the only ones that exist at H&M when building applications and you will see that we frequently link to other guidelines, principles and requirements. See them as a practical guide on how to deliver on some of the capabilities in Technology Foundation. Technology Foundation refers to the architecture capabilities we need to have in place to meet the IT2020 strategy and is a part of the H&M Group Key Development Areas for 2017.

We strongly promote these guidelines when building new applications or making changes to existing ones. But the guidelines are not principles since not all of them are relevant in every situation, but if it's decided not to follow a guideline you should seek formal approval from relevant stakeholders on division or group level with the architecture positioning process.

## General Service Design Guidelines

* All services should be reachable over the internet (publicly routed network) (Link to "How to publish your app on the internet -> How to secure your app  ie WAF"). We are striving to increase mobility and internet reachability is a key enabler.
* Always use encryption of data in network transit according to (Link to page About Certificates/TLS/SSL --> Crypto Guidelines). Example: Use TLS (https) when transmitting data between the client and the server.
* HTTPS (or other internet safe protocols) should be the only protocol used when clients communicate with backend services
* "API:er"
* Host your application in generally available IaaS or PaaS services as first choice, but analyse if the architecture of the application is a good fit for cloud. (Link to "How to host your application").
* We are a global company, analyse where your users are and use CDN and/or geo-replication services available from our cloud providers if necessary. (Link to "Patterns for global deployment of services").
* Use standard platform services for data storage (databases, files, etc) that is generally available from our cloud providers instead of installing and managing on services on servers. (Link "Storage Services")
* https://aws.amazon.com/blogs/aws/well-architected-working-backward-to-play-it-forward/


## Access and Identity Guidelines

* Use our central identity service for authenticating internal (employees etc) users with SAMLv2, OAuth2 or Open ID. (Link to page about Authenticating users) (https://www.mutuallyhuman.com/blog/2013/05/09/choosing-an-sso-strategy-saml-vs-oauth2/)
* Always use use two factor authentication (MFA) for authenticating users (Link to page about Authenticating users)
* (APIs and IAM, link to IAM guidelines) 
* (External Users and Partners B2B authentication)

## Client Design Guidelines

* End user applications should be build using HTML5 / JavaScript / CSS and not rely on any browser plugins (link to "Client Design guidelines").
* Applications should be developed with mobile devices in mind (phones and tablets) and be responsive (link to "Client Design guidelines").
* Standard H&M browsers should be supported for browser based applications (link to Standard Browsers).
* Non browser based applications (fat clients etc) should only be used when they offer productivity improvements for the end users.
* When native mobile applications are built, a framework that relies on web technologies like Apache Cordova is recommended to lower the cost of cross platform development.


## Integration

* API:s etc… 
* Versioning…
* Public end-points
* Application to Application Identity and Security

## Monitoring
