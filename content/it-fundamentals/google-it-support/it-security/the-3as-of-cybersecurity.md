---
title: 'The 3As of Cybersecurity - 3A Authentication, Authorization, Accounting'
linkTitle: The 3As of Cybersecurity
date: 2022-10-13 07:46:00 +0500
weight: 3
collapsibleMenu: true
alwaysOpen: false
LastModifierDisplayName: AbuTurab
LastModifierEmail: cyberfrontofficial@proton.me
---

## **Authentication**

Three types of authentication methods:
+ Something you know – password or pin
+ Something you have – bank card, USB device, key fob, or OTP
+ Something you are – biometric data, like a fingerprint, voice signature, facial recognition, or retinal scan

Some additional categories of authentication methods:
+ Somewhere you are – geofencing, GPS, Indoor Positioning Systems (IPS)
+ Something you do – gestures, swipe patterns, CAPTCHA, or patterns of behavior

### **Authentication Best Practices**
  
  Incorporating **good password policies** into an organization is key to ensuring that employees are securing their accounts with **strong passwords**.
  
  A good password practice makes sure of:
  + Length requirements
  + Character complexity
  + Dictionary words

#### Identification
  
  The idea of describing an entity uniquely.

### **Multifactor Authentication**
  
  A system where users are authenticated by presenting multiple pieces of information or objects.
  + OTP with physical token
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity.png)
  
  + Counter-based token
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-1.png)
  
  + Biometrics
  + U2F – Universal 2nd Factor
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-2.png)

#### Biometric authentication
  
  The process of using unique physiological characteristics of an individual to identify them.
  
  **They're [creating fake fingerprints using things like glue](https://www.hindustantimes.com/mumbai-news/you-will-be-glued-to-this-mumbai-college-s-students-trick-biometric-system/story-W64f1jdMtecxKDml2DakeI.html), allowing friends to mark each other as present if they're late or skip school**.

### **Certificates**
  
  In order to issue client certificates, an organization must set up and maintain CA infrastructure to issue and sign certificates.
  
  The certificates are checked against CRL.

#### Certificate revocation list (CRL)
  
  A signed list published by the CA which defines certificates that have been explicitly revoked.

### LDAP
  
  Lightweight Directory Access Protocol (LDAP) is an open, industry-standard protocol for accessing and maintaining directory services.
  + Bind: How clients authenticate to the server.
  + StartTLS: It permits a client to communicate using LDAP v3 over TLS
  + Search: For performing look-ups and retrieval of records.
  + Unbind: It closes the connection to the LDAP server.

### RADIUS
  
  Remote Authentication Dial-In User Service (RADIUS) is a protocol that provides AAA services for users on a network.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-3.png)

### Kerberos
  
  A network authentication protocol that uses “tickets” to allow entities to prove their identity over potentially insecure channels to provide mutual authentication.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-4.png)

### TACACS+
  
  Terminal Access Controller Access-Control System Plus
  + TACACS+ is primarily used for device administration, authentication, authorization, and accounting.

### **Single Sign-On**
  
  An authentication concept that allows users to authenticate once to be granted access to a lot of different services and applications.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-5.png)

#### OpenID
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-6.png)

## **Authorization**
  
  Pertains to describing what the user account has access to, or doesn't have access to.

### Authorization and Access Control Methods
  
  One popular and open standard for authorization is:
  + OAuth

### **Access Control**

#### OAuth
  
  An open standard that allows users to grant third-party websites and applications access to their information without sharing account credentials.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-7.png)
  
  + OAuth's permissions can be used in phishing-style attacks to again access to accounts, **without requiring credentials** to be compromised.
  
  **This was used in an [OAuth-based worm-like attack](https://www.theverge.com/2017/5/3/15534768/google-docs-phishing-attack-share-this-document-with-you-spam) in early 2017, with a rash of phishing emails that appeared to be from a friend or colleague who wants to share a Google Document**.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-8.png)

### Access Control List (ACL)
  
  A way of defining permissions or authorization for objects.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-9.png)

## **Accounting**
  
  Keeping records of what resources and services your users accessed, or what they did when they were using your systems.
  + Auditing

### Tracking Usage and Access
  
  What exactly accounting tracks, depends on the purpose and intent of the system.
  + A TACACS+ server would be more concerned with keeping track of user authentication, what systems they authenticated to, and what commands they ran during their session.
  
  TACACS+ is a devices access AAA system that manages who has access to your network devices and what they do on them.
  + CISCO's AAA system supports accounting of individual commands executed, connection to and from network devices, commands executed in privileged mode, and network services and system details like configuration reloads or reboots.
  + RADIUS will track details like session duration, client location and bandwidth, or other resources used during the session.
  
  ![The 3As of Cybersecurity](/notes/google-it-support/the-3as-of-cybersecurity-10.png)
  
  RADIUS accounting can be used by ISPs to charge for their services.
