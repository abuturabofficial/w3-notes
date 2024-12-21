---
title: "Scanning"
date: 2023-04-28 11:01:00 +0500
LastModifierDisplayName: AbuTurab
LastModifierEmail: cyberfrontofficial@proton.me
collapsibleMenu: true
alwaysOpen: false
weight: 3
---

## **Vulnerability Assessment Tools**
  
  “Vulnerability scanning identifies hosts and host attributes (e.g., OSs, applications, open ports), but it also attempts to identify vulnerabilities rather than relying on human interpretation of the scanning results. Vulnerability scanning can help identify outdated software versions, missing patches, and misconfigurations, and validate compliance with or deviation from an organization’s security policy.”  **— NIST SP 800-115**

### **What is a Vulnerability Scanner?**
  
  **Capabilities:**
- Keeping an up-to-date database of vulnerabilities.
- Detection of genuine vulnerabilities without an excessive number of false positives.
- Ability to conduct multiple scans at the same time.
- Ability to perform trend analyses and create clear reports of the results.
- Provide recommendations for effective countermeasures to eliminate discovered vulnerabilities.

#### Components of Vulnerability Scanners
  
There are 4 main components of most scanners:
1. **Engine Scanner**
  - Performs security checks according to its installed plug-ins, identifying system information, and vulnerabilities.
1. **Report Module**
  - Provides scan result reporting such as technical reports for system administrators, summary reports for security managers, and high-level graph and trend reports for corporate executives' leadership.
1. **Database**
  - Stores vulnerability information, scan results, and other data used by the scanner.
1. **User interface**
  - Allows the admin to operate the scanner. It may be either a GUI, or just a CLI.

#### Host & Network
  
  **Internal Threats:**
- It can be through Malware or virus that is downloaded onto a network through internet or USB.
- It can be a disgruntled employee who has the internal network access.
- It can be through the outside attacker who has gained access to the internal network.
- The internal scan is done by running the vulnerability scanner on the critical components of the network from a machine which is a part of the network. This important component may include core router, switches, workstations, web server, database, etc.
  
  **External Threats:**
- The external scan is critical as it is required to detect the vulnerabilities to those internet facing assets through which an attacker can gain internal access.

#### Common Vulnerability Scoring Systems (CVSS)
  
  The CVSS is a way of assigning severity rankings to computer system vulnerabilities, ranging from zero (least severe) to 10 (most severe).
- It provides a standardized vulnerability score across the industry, helping critical information flow more effectively between sections within an organization and between organizations.
- The formula for determining the score is public and freely distributed, providing transparency.
- It helps prioritize risk — CVSS rankings provide both a general score and more specific metrics.
  
![Scanning](/notes/Scanning.png)

**Score Breakdown:**

The CVSS score has three values for ranking a vulnerability:
1. **A base score**, which gives an idea of how easy it is to exploit targeting that vulnerability could inflict.
2. **A temporal score**, which ranks how aware people are of the vulnerability, what remedial steps are being taken, and whether threat actors are targeting it.
3. **An environmental score**, which provides a more customized metric specific to an organization or work environment.

![Scanning](/notes/Scanning-1.png)

### STIGS – Security Technical Implementation Guides

- The Defense Information Systems Agency (DISA) is the entity responsible for maintaining the security posture of the DoD IT infrastructure.
- Default configurations for many applications are inadequate in terms of security, and therefore DISA felt that developing a security standard for these applications would allow various DoD agencies to utilize the same standard – or STIG – across all application instances that exist.
- STIGs exist for a variety of software packages including OSs, DBAs, OSS, Network devices, Wireless devices, Virtual software, and, as the list continues to grow, now even include Mobile Operating Systems.

### Center for Internet Security (CIS)
  
  **Benchmarks:**
- CIS benchmarks are the only consensus-based, best-practice security configuration guides both developed and accepted by government, business, industry, and academia.
- The initial benchmark development process defines the scope of the benchmark and begins the discussion, creation, and testing process of working drafts. Using the CIS WorkBench community website, discussion threads are established to continue dialogue until a consensus has been reached on proposed recommendations and the working drafts. Once consensus has been reached in the CIS Benchmark community, the final benchmark is published and released online.
  
  **Controls:**
  The CIS Controls<sup>TM</sup> are a prioritized set of actions that collectively form a defense-in-depth set of best practices that mitigate the most common attacks against systems and networks. The CIS Controls are developed by a community of IT experts who apply their first-hand experience as cyber defenders to create these globally accepted security best practices.
  
  The five critical tenets of an effective cyber defense systems as reflected in the CIS Controls are:
  1. Offense informs defense
  2. Prioritization
  3. Measurements and metrics
  4. Continuous diagnostics and mitigation
  5. Automation

### **Implementation Groups**
  
![Scanning](/notes/Scanning-2.png)

#### 20 CIS Controls
  
![Scanning](/notes/Scanning-3.png)

## **Port Scanning**
  
“Network port and service identification involves using a port scanner to identify network ports and services operating on active hosts–such as FTP and HTTP–and the application that is running each identified service, such as Microsoft Internet Information Server (IIS) or Apache for the HTTP service. All basic scanners can identify active hosts and open ports, but some scanners are also able to provide additional information on the scanned hosts.” —**NIST SP 800-115**

### Ports

- Managed by IANA.

### Responses

- A port scanner is a simple computer program that checks all of those doors – which we will start calling ports – and responds with one of three possible responses:
  1. Open — Accepted
  2. Close — Not Listening
  3. Filtered — Dropped, Blocked

### **Types of Scans**
  
Port scanning is a method of determining which ports on a network are open and could be receiving or sending data. It is also a process for sending packets to specific ports on a host and analyzing responses to identify vulnerabilities.

1. **Ping:**
  - Simplest port scan sending ICMP echo request to see who is responding
1. **TCP/Half Open:**
  - A popular, deceptive scan also known as SYN scan. It notes the connection and leaves the target hanging.
1. **TCP Connect:**
  - Takes a step further than half open by completing the TCP connection. This makes it slower and noisier than half open.
1. **UDP:**
  - When you run a UDP port scan, you send either an empty packet or a packet that has a different payload per port, and will only get a response if the port is closed. It's faster than TCP, but doesn’t contain as much data.
1. **Stealth:**
  - These TCP scans are quieter than the other options and can get past firewalls. They will still get picked by the most recent IDS.

#### Tools – NMAP
  
  NMAP (Network Mapper) is an open source tool for network exploration and security auditing.
- Design to rapidly scan large networks, though work fine against single hosts.
- Uses raw IP packets.
- Used to know, service type, OS type and version, type of packet filter/firewall in use, and many other things.
- Also, useful for network inventory, managing service upgrade schedules, and monitoring host or service uptime.
- ZenMap is a GUI version of NMAP.

## **Network Protocol Analyzers** 
  
  “A protocol analyzer (also known as a **sniffer, packet analyzer, network analyzer, or traffic analyzer**) can capture data in transit for the purpose of analysis and review. Sniffers allow an attacker to inject themselves in a conversation between a digital source and destination in hopes of capturing useful data.”

### **Sniffers**
  
  Sniffers operate at the data link layer of the OSI model, which means they don’t have to play by the same rules as the applications and services that reside further up the stack. Sniffers can capture everything on the wire and record it for later review. They allow user’s to see all the data contained in the packet.
- Wireshark
  
![Scanning](/notes/Scanning-4.png)

#### WireShark
  
  Wireshark intercepts traffics and converts that binary traffic into human-readable format. This makes it easy to identify what traffic is crossing your network, how much of it, how frequently, how much latency there is between certain hops, and so on.
- Network Admins use it to troubleshoot network problems.
- Network Security Engineers use it to examine security issues.
- QA engineers use it to verify network applications.
- Developers use it to debug protocol implementations.
- People use it to learn network protocol internals.

##### WireShark Features

- Deep inspection of hundred of protocols, with more being added all the time
- Live capture and offline analysis
- Standard three pane packet browser
- Cross-platform
- GUI or TTY-mode – TShark utility
- Powerful display filters
- Rich VoIP analysis
- Read/write to different formats
- Capture compressed file with gzip
- Live data from any source
- Decryption support for many protocols
- Coloring rules
- Output can be exported to different formats

#### Packet Capture (PCAP)
  
  PCAP is a valuable resource for file analysis and to monitor network traffic.
- Monitoring bandwidth usage
- Identify rogue DHCP servers
- Detecting Malware
- DNS resolution
- Incident Response
  
  Wireshark is the most popular traffic analyzer in the world. Wireshark uses `.pcap` files to record packet data that has been pulled from a network scan. Packet data is recorded in files with the `.pcap` file extension and can be used to find performance issues and cyberattacks on the network.
  
![Scanning](/notes/Scanning-5.png)

# **Security Architecture considerations**

## **Characteristics of a Security Architecture**
  
  **The foundation of robust security is a clearly communicated structure with a systematic analysis of the threats and controls.**
- Build with a clearly communicated structure
- Use systematic analysis of threats and controls
  
  **As IT systems increase in complexity, they require a standard set of techniques, tools, and communications.**
  
  **Architectural thinking is about creating and communicating good structure and behavior with the intent of avoiding chaos.**
  
  Architecture need to be:
- Described before it can be created
- With different level of elaboration for communication
- Include a solution for implementation and operations
- That is affordable
- And is secure
  
> Architecture: “The architecture of a system describes its overall static structure and dynamic behavior. It models the system’s elements (which for IT systems are software, hardware and its human users), the externally manifested properties of those elements, and the static and dynamic relationships among them.”

> ISO/IEC 422010:20071 defines Architecture as “the fundamental organization of a system, embodied in its components, their relationships to each other and the environment, and the principles governing its design and evolution.”

## **High-level Architectural Models**
  
**Enterprise and Solution Architecture break down the problem, providing different levels of abstraction.**
  
![Scanning](/notes/Scanning-6.png)
  
**High-level architectures are described through Architectural Building Blocks (ABBs) and Solution Building Blocks (SBBs).**
  
![Scanning](/notes/Scanning-7.png)
  
**Here are some example Security ABBs and SBBs providing different levels of abstraction aimed at a different audience.**
  
![Scanning](/notes/Scanning-8.png)
  
**Here is a high level example of an Enterprise Security Architecture for hybrid multicloud showing security domains.**

![Scanning](/notes/Scanning-9.png)

**The Enterprise Security Architecture domains could be decomposed to show security capabilities… without a context.**

![Scanning](/notes/Scanning-10.png)

**Adding context gives us a next level Enterprise Architecture for hybrid multi-cloud, but without specific implementation.**

![Scanning](/notes/Scanning-11.png)

## **Solution Architecture**
  
**Additional levels of abstraction are used to describe architectures down to the physical operational aspects.**

![Scanning](/notes/Scanning-12.png)

**Start with a solution architecture with an Architecture Overview giving an overview of the system being developed.**

![Scanning](/notes/Scanning-13.png)

**Continue by clearly defining the external context describing the boundary, actors and use that process data.**

![Scanning](/notes/Scanning-14.png)

**Examine the system internally looking at the functional components and examine the threats to the data flows.**

![Scanning](/notes/Scanning-15.png)

**Finally, look at where the function is hosted, the security zones and the specific protection required to protect data.**

![Scanning](/notes/Scanning-16.png)

**As the architecture is elaborated, define what is required and how it will be delivered?**

![Scanning](/notes/Scanning-17.png)

## **Security Patterns**

**The use of security architecture patterns accelerate the creation of a solution architecture.**

A security Architecture pattern is
- a reusable solution to a commonly occurring problem
- it is a description or template for how to solve a problem that can be used in many different situations
- is not a finished design as it needs conext
- it can be represented in many different formats
- Vendor specific or agnostic
- Available at all levels of abstraction

![Scanning](/notes/Scanning-18.png)
  
  **There are many security architecture patterns available to provide a good starting point to accelerate development.**

# **Application Security Techniques and Risks**

## **Application Security Overview**
  
![Scanning](/notes/Scanning-19.png)

### Software Development Lifecycle

![Scanning](/notes/Scanning-20.png)

### Penetration Testing Tools

![Scanning](/notes/Scanning-21.png)

### Source Code Analysis Tools

![Scanning](/notes/Scanning-22.png)

## **Application Security Threats and Attacks**

### Third Party Software

- Standards
- Patching
- Testing
  
  **Supplier Risk Assessment**
- Identify how any risks would impact your organization's business. It could be a financial, operational or strategic risk.
- Next step would be to determine the likelihood the risk would interrupt the business
- And finally there is a need to identify how the risk would impact the business.

### Web Application Firewall (WAF)
  
![Scanning](/notes/Scanning-23.png)

### Application Threats/Attacks
  
  **Input Validation:**
- Buffer overflow
- Cross-site scripting
- SQL injection
- Canonicalization
  
  **Authentication:**
- Network eavesdropping
- Brute force attack
- Dictionary attacks
- Cookie replay
- Credential theft
  
  **Authorization:**
- Elevation of privilege
- Disclosure of confidential data
- Data tampering
- Luring Attacks
  
  **Configuration Management:**
- Unauthorized access to admin interface
- Unauthorized access to configuration stores
- Retrieval of clear text configuration data
- Lack of individual accountability; over-privileged process and service accounts
  
  **Exception Management:**
- Information disclosure
- DoS
  
  **Auditing and logging:**
- User denies performing an operation
- Attacker exploits an application without trace
- Attacker covers his tracks

## **Application Security Standards and Regulations**

### Threat Modeling
  
  “Threat modeling is a process by which potential threats, such as structural vulnerabilities or the absence of appropriate safeguards, can be identified, enumerated, and mitigations can be prioritized.”
  
  Conceptually, a threat modeling practice flows from a methodology.
1. **STRIDE methodology**: STRIDE is a methodology developed by Microsoft for threat modeling. It provides a mnemonic for security threats in six categories: Spoofing, Tampering, Repudiation, Information disclosure, Denial of service and Elevation of privilege.
  - Microsoft developed it
1. **P.A.S.T.A:** P.A.S.T.A. stands for Process for Attack Simulation and Threat Analysis. It is an attacker-focused methodology that uses a seven-step process to identify and analyze potential threats.
  - Seven-step process
1. **VAST:** VAST is an acronym for Visual, Agile, and Simple Threat modeling. The methodology provides actionable outputs for the unique needs of various stakeholders like application architects and developers.
2. **Trike:** Trike threat modeling is an open-source threat modeling methodology focused on satisfying the security auditing process from a cyber risk management perspective. It provides a risk-based approach with unique implementation and risk modeling process.

### Standards vs Regulations
  
  | Standards                         | Regulations              |
  | --------------------------------- | ------------------------ |
  | Cert Secure Coding                |                          |
  | Common Weakness Enumeration (CWE) | Gramm-Leach-Bliley Act   |
  | DISA-STIG                         | HIPAA                    |
  | ISO 27034/24772                   | Sarbanes-Oxley Act (SOX) |
  | PCI-DSS                           |                          |
  | NIST 800-53                       |                          |

## **DevSecOps Overview**

### Why this matter?
  
![Scanning](/notes/Scanning-24.png)

- Emerging DevOps teams lead to conflicting objectives.
- DevSecOps is an integrated, automated, continuous security; always.
  
  **Integrating Security with DevOps to create DevSecOps.**
  
![Scanning](/notes/Scanning-25.png)

### **What does DevSecOps look like?**
  
![Scanning](/notes/Scanning-26.png)

- Define your operating and governance model early.
- A successful program starts with the people & culture.
	- Training and Awareness
	- Explain and embrace new ways of working
	- Equip teams & individuals with the right level of ownership & tools
- Continuous improvement and feedback.

#### Develop Securely: Plan A security-first approach
  
  Use tools and techniques to ensure security is integral to the design, development, and operation of all systems.
  
  Enable empowerment and ownership by the Accreditor/Risk owner participating in Plan & Design activities.
  
  **Security Coach** role to drive security integration.
  
![Scanning](/notes/Scanning-27.png)

![Scanning](/notes/Scanning-28.png)

#### Develop Security: Code & Build Security & Development combined
  
  Apply the model to Everything-as-Code:
- Containers
- Apps
- Platforms
- Machines
- Shift security to the left and embrace security-as-code.
- Security Engineer to drive technical integration and uplift team security knowledge.
  
  
![Scanning](/notes/Scanning-29.png)

#### Develop Securely: Code & Build
  
  Detect issues and fix them, earlier in the lifecycle
  
![Scanning](/notes/Scanning-30.png)

#### Develop Securely: Test
  
  Security and development Combined
  
![Scanning](/notes/Scanning-31.png)
  
  Validate apps are secure before release & development.
  
![Scanning](/notes/Scanning-32.png)

## **DevSecOps Deployment**

### Secure Operations: Release, Deploy & Decom
- Orchestrate everything and include security.
- Manage secure creation and destruction of your workloads.
- Automate sign-off to certified levels of data destruction.
  
Controlled creation & destruction
  
![Scanning](/notes/Scanning-33.png)

Create securely, destroy securely, every time.

![Scanning](/notes/Scanning-34.png)

### **Secure Operations: Operate & Monitor**

- If you don’t detect it, you can’t fix it.
- Integrated operational security helps ensure the security health of the system is as good as it can be with the latest information.
- Playbooks-as-code run automatically, as issues are detected they are remediated and reported on.
  
  Security & Operations combined
  
![Scanning](/notes/Scanning-35.png)
  
  It’s not a question of if you get hacked, but when.
  
![Scanning](/notes/Scanning-36.png)

#### So, why DevSecOps?
  
![Scanning](/notes/Scanning-37.png)

# **Deep Dive into Cross-Site Scripting**

## **Application Security Defects – Writing Secure Code**

### What, Should I worry?
  
![Scanning](/notes/Scanning-38.png)

### Issues Types

- Majority of security products have Web UIs: LMIs, Administrative Interfaces, Dashboards.
- Web vulnerabilities most commonly reported by 3rd parties as well as internal pen-testers, with XSS far in the lead.
- Crypto vulnerabilities come next.
- Appliances highly susceptible to command execution vulnerabilities.

### Writing Secure Software is Not Easy

- Developers face many challenges:
  
![Scanning](/notes/Scanning-39.png)

- Yet with good security education, and solid design and implementation practices, we can make sure our products are secure.

### Mitigating Product Security Risk

- Prevent new bugs
	- SANS 25 most dangerous programming errors.
- Think like a hacker.
- Build defenses in your software.
	- Input Validation
	- Output Sanitization
	- Strong encryption
	- Strong Authentication & Authorization
- Choose secure frameworks rather than simply rely on developer security skills.
- Don’t think that if your product is isolated from the Internet, it isn’t at risk.
- Don’t think that if a file or database is local, it doesn’t need to be protected. The majority of breaches are launched from INSIDE.
- Address existing bugs.
	- Redesign for not only looks, but for security and functionality.
	- Implement smart architectural changes that fix security flaws at the top.
	- Don’t spot-fix issues, think of how the vulnerability can be fixed across the board and prevented in the future.
	- Security bugs are special. (Need to be fixed asap)
		- Deliver security patches with faster release vehicles.

## **Cross scripting – Common Attacks**
  
  Cross-Site Scripting (XSS)
- Allows attackers to inject client-side scripts into the Web Page
- Can come from anywhere:
	- HTTP parameters
	- HTTP headers and cookies
	- Data in JSON and XML files
	- Database
	- Files uploaded by users
- Most common security issues found in many security products.

### Dangers of XSS

- Harvest credentials
- Take over user sessions
- CSFR
- Steal cookies, local store data
- Elevate privileges
- Redirect users to malicious sites

## **Cross-site Scripting – Effective Defenses**

- Preventing XSS with HTML Encoding
	- Enforcing the charset (UTF-8)
- Preventing XSS with JS Escaping
	- Escaping single quotes will prevent injection
	- Preventing XSS by using safe DOM elements
	- Use Eval and Dynamic Code Generation with Care
- Input Validation
	- Whitelisting – recommended
	- Blacklisting – not recommended
	- Client Side input validation – not recommended
	- Use proven Validation and Encoding Functionality
