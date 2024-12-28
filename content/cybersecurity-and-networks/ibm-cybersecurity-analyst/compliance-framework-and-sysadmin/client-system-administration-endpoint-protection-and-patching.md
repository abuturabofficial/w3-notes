---
title: "Client System Administration Endpoint Protection and Patching"
linkTitle: Client SysAdmin Endpoint
date: 2023-03-11 12:40:00 +0500
LastModifierDisplayName: AbuTurab
LastModifierEmail: cyberfrontofficial@proton.me
collapsibleMenu: true
alwaysOpen: false
weight: 2
---

## **Client System Administration**

“The client-server model describes how a server provides resources and services to one or more clients. Examples of servers include web servers, mail servers, and file servers. Each of these servers provide resources to client devices, such as desktop computers, laptops, tablets, and smartphones. Most servers have a one-to-many relationship with clients, meaning a single server can provide resources to multiple clients at one time.”

### Client System Administration

- Cloud and Mobile computing
- New Devices, new applications and new services.
- Endpoint devices are the front line of attack.

### Common type of Endpoint Attacks

- **Spear Phishing/Whale Hunting** – An email imitating a trusted source designed to target a specific person or department.
- **Watering Hole** – Malware placed on a site frequently visited by an employee or group of employees.
- **Ad Network Attacks – Using ad networks to place malware on a machine through ad software.
- **Island Hopping** – Supply chain infiltration.

## **Endpoint Protection**

### Basics of Endpoint Protection

- Endpoint protection management is a policy-based approach to network security that requires endpoint devices to comply with specific criteria before they are granted access to network resources.
- Endpoint security management systems, which can be purchased as software or as a dedicated appliance, discover, manage and control computing devices that request access to the corporate network.
- Endpoint security systems work on a client/server model in which a centrally managed server or gateway hosts the security program and an accompanying client program is installed on each network devices.

### Unified Endpoint Management
  
  A UEM platform is one that converges client-based management techniques with Mobile device management (MDM) application programming interfaces (APIs).

## **Endpoint Detection and Response**
  
  **Key mitigation capabilities for endpoints**
- Deployment of devices with network configurations
- Automatic quarantine/blocking of non-compliant endpoints
- Ability to patch thousands of endpoints at once
  
  **Endpoint Detection and Response**
- Automatic policy creation for endpoints
- Zero-day OS updates
- Continuous monitoring, patching, and enforcement of security policies across endpoints.

### Examining an Endpoint Security Solution
  
  Three key factors to consider:
  1. Threat hunting
  2. Detection response
  3. User education

# **An Example of Endpoint Protection**

## **Unified Endpoint Management**
  
  UEM is the first step to enable today’s enterprise ecosystem:
- Devices and things
- Apps and content
- People and identity

### What is management without insight?
  
  IT and security needs to understand:
- What happened
- What can happen
- What should be done
  … in the context of their environment

### **Take a new approach to UEM**
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching.webp)

#### UEM with AI
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching-1.webp)
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching-2.webp)

### **Traditional Client Management Systems**

- Involves an agent-based approach
- Great for maintenance and support
- Standardized rinse and repeat process
- Applicable for some OS & servers

#### Mobile Device Management

- API-based management techniques
- Security and management of corporate mobile assets
- Specialized for over-the-air configuration
- Purpose-built for smartphones and tablets

### Modern Unified Endpoint Management
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching-3.webp)
  
  IT Teams are also converging:
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching-4.webp)

## **Overview of Patching**

- All OS require some type of patching.
- Patching is the fundamental and most important thing an organization can do to prevent malicious attacks.

### What is a patch?
  
  A patch is a set of changes to a computer program or its supporting data designed to update, fix, or improve it. This includes fixing security vulnerabilities and other bugs, with such patches usually being called bugfixes, or bug fixes, and improving the functionality, usability or performance.

## **Windows Patching**

- Windows Updates allow for fixes to known flaws in Microsoft products and OS. The fixes, known as patches, are modification to software and hardware to help improve performance, reliability, and security.
- Microsoft releases patches in a monthly cycle, commonly referred to as “Patch Tuesday”, the second Tuesday of every month.

### Four types of Updates for Windows OSes
  
  1. **Security Updates:** Security updates for Windows work to protect against new and ongoing threats. They are classified as Critical, Important, Moderate, Low, or non-rated.
  2. 590344 These are high priority updates. When these are released, they need to updated asap. It is recommended to have these set as automatic.
  3. **Software Updates:** Software updates are not critical. They often expand features and improve the reliability of the software.
  4. **Service Packs:** These are roll-ups, or a compilation, of all previous updates to ensure that you are up-to-date on all the patches since the release of the product up to a particular data. If your system is behind on updates, then service packs bring your system up-to-update.

## **Windows Application Patching**
  
  **Why patch 3<sup>rd</sup> party applications in addition to Windows OS?**
- Unpatched software, especially if a widely used app like Adobe Flash or Browser, can be a magnet for malware and viruses.
- **87%** of the vulnerabilities found in the top 50 programs affected third-party programs such as Adobe Flash and Reader, Java, Skype, Various Media Players, and others outside the Microsoft Ecosystem. That means the remaining 13 percent “stem from OSes and Microsoft Programs,” according to Secunia’s Vulnerability Review report.

### Patching Process
  
  ![Client System Administration Endpoint Protection and Patching](/notes/ibm-cybersecurity-analyst/Client%20System%20Administration%20Endpoint%20Protection%20and%20Patching-5.webp)
