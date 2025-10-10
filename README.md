## Computer Networking

### What is computer networking?

Computer networking is known for communication between computer devices (computer, printers) by exchanging information between them.

It works both wired and wireless methods through wired mode like ethernet cables and wireless like bluetooth, wi-fi or nearby sharing.

---

### LAN (Local Area Network)

![Lan Diagram](/assets/lan.png)

Computer network that interconnects all the computer devices in a **limited area**.

Example: School, hospital, college.

### WAN (Wide Area Network)

![Wan Diagram](/assets/wan.png)

It is a computer network that interconnects all the computers across the different geographical locations using **Public network or Internet**.

Note: LAN is a subset of WAN.

Example: Let's say each LAN from the diagram refers to different locations to connect all these LAN to one network Internet is used which is WAN.

### MAN (Metropolitan Area Network)

It is a computer network that connects all computer devices within a city or metro station using public network or internet.

Note: LAN is a subset of MAN.

### Log

Computer recorded activity.

![Log Event Viewer Diagram](/assets/log.png)

If you search for **event viewer** on your laptop you can see all logs that will be running in the backend right from the laptop switched on. Event ID **4624** is for user login successfully on the laptop which records each and every that user performed on his laptop.

Example: Windows laptop logs

Application, Audit or Security, System, Config

All the above logs will be integrated to SIEM tool using different log integration methods.

---

### SIEM (Security Information and Event Management)

#### Log Collection

Collects all logs from the employees systems or application logs or security logs.

#### Log Processing

Processing the logs.

#### Log Analysis

Analysis will be done my security analyst if there is any abnormal activities happen.

#### Log Monitoring

It is done by SIEM TOOL.

#### Incident alert notification generation

Any hacking or any malicious activity happen SIEM will give alerts via email for L1,L2,L3 team we have to do instant investigation.

---

### SOC (Security Operation Center)

It is a dedicated site or room where cyber security analyst (L1,L2,L3 with SOC Manager) will seat and monitor 24*7*365 days and when ever any security incidents or alerts will come they will take care incident investigation or Forensic investigation.

### DC (Data Center (On premise))

This is a site or room where data is stored just like servers in one place. It has to be stores in good temperature condition providing ventilation as well.

### DC (Domain Controller)

Domain Controller is nothing but centralized authentication and authorization of a server. IT team or service desk team will be taking responsibility regarding this management. When a employee facing any issue like they are unable to reach a specific domain or access that domain which will be available for few teams they have to reach out to this team so that they will resolve this issue.

### Authentication

Trying to login with credentials to a server, data base, application with valid username and password.

Note: Authentication provides identification of the user **WHO AM I**.

### Authorization

Validating the credentials whether they have access to that particular website, application, server or data base.

Note: Authorization is always provide from backed server **WHO ARE YOU**.

---

### CIA (Confidentiality, Integrity, Availability)

#### Confidentiality

Keeping data or information safe by giving access to only authorized users.

#### Integrity

Checking the file properties like who has the access to modifying the data like adding or deleting files.

#### Availability

Availability of a application to end user without any business outage.
Because if we take amazon as example for one minutes if the app is not functioning properly or app not available to the end user then it would be huge loss to the company. So, application should be 99.99999% available for the end user or customers.

---

### Encryption

Converting plain text to encrypted data using Encryption methods or **password or key**.

### Decryption

Converting encrypted data to plain text using decryption methods or **password or key**.

### Compression

Decreasing the size of file with or without loosing the information within the file.

Lossless File: PNG, FLAC, ZIP

Lossy File: MP3, JPEG

### Decompression

Restoring back from the compressed file.

### Encoding

Converting one form of data into another.

### Decoding

Converting encoded data back to the original.

---

### ARP (Address Resolution Protocol)

It is process of converting layer 3 (IP address - used in Network layer in [OSI layers](#osi-layers)) to layer 2 (MAC address - used in Data Link Layer in OSI Layers)

![ARP Real-time example](/assets/arp.png)

As here you can see IP address to physical address which is also MAC address.

### RARP (Reverse Address Resolution Protocol)

It is process of converting layer 2 (MAC address - used in Data Link Layer in OSI Layers) to layer 3 (IP address - used in Network layer in [OSI layers](#osi-layers)).

### FIREWALL

Process of monitoring [in bound](#in-bound-traffic) and [out bound traffic](#out-bound-traffic) on the basis of set of rules it will either allow or deny.

### SMTP server (Simple Mail Transfer Protocol)

Used for sending and receiving mails. It is also known as Exchange server or email server.

### Traffic

It is flow of data as packets.

#### In bound traffic

Traffic coming from outside to inside is known as in bound traffic.

Example: In TCS perspective if you try to apply any job you will be external person so there will be inbound traffic for TCS as your are trying to reach TCS domain to apply.

#### Out bound traffic

Traffic going from inside to outside is known as out bound traffic.

Example: In TCS perspective if you try to use google docs which is external for TCS, trying to upload a file or managing a file from TCS which is know as out bound traffic because traffic going from TCS to Google Docs.

### Netflow data

It is combination of both [in bound](#in-bound-traffic) and [out bound traffic](#out-bound-traffic). Net flow is provided by Cisco. It is available in Cisco router and switches. There are HP and IBM router, servers as well but they are not net data flow.

Even Netflow data should be integrated to SIEM tool in the form of IP packets.

### Abnormal or Suspicious or Malicious

Harmful for the organizations server.

### Attackers or Hackers or Threat actor or Intruder or Adversary

When a person try to hack unauthorized access or sensitive exposure for the sake of money is known as hacker.

### Vulnerability

It is weakness in a system.

Example: System mean we are not just referring to computers or devices it could be organization or application or data base or servers.

### Threat

If a hacker try to exploit vulnerability it is known as threat.

### Risk

Vulnerability \* Threat

[Likelihood](#likelihood) \* [Impact](#impact)

Destruction of the damage is also know as risk.

### Likelihood

How often this attack or chaos occur in a span of one year.

### Impact

What are all the consequences for the Likelihood.

---

### OSI Layer (Open System Interconnection)

Establishing communication between devices by following few protocols.

### 7 Application Layer

It is the top most layer in OSI layer which provides network to the end user for communicating directly with the application or website.

Website: HTTP(80), HTTPS(443)

Messaging: SMTP - Simple Mail Transfer Protocol (25) used for sending and receiving messages, Pop 3 - Post Office Protocol (110) used for downloading messages to local folder, IMAP - Internet Message Access Protocol (143) used to manage the messages or organizing, ICMP - Internet Control Message Protocol,
Terminal: SSH - Secure Shell (22), RDP - Remote Desktop Protocol (3389)

File Transfer:: FTP - File Transfer Protocol (20,21), SFTP - Secure File Transfer Protocol (22), NFS - Network File Sharing

DNS - Domain Name System (53), DHCP - Domain Host Configure Protocol (67,68),

### 6 Presentation Layer

Process of converting one form data into another.

![Encryption](#encryption), ![Decryption](#decryption)

![Compression](#compression), ![Decompression](#decompression)

![Encoding](#encoding), ![Decoding](#decoding)

### 5 Session Layer

Managing the session between client and server.

Session Management

![Authentication](#authentication)

![Authorization](#authorization)

### 4 Transport Layer

Here the data will be transferred from source ip to destination ip with error flow control and data flow.

#### Segmentation

Dividing large chunk of data into small chunks.

#### Error Flow Control

Transferring data in a sequence order with our error.

#### Data Flow Control

Controls the speed of transferring data.

#### TCP 3 way handshake

---

#### Network Diagram

![Network Diagram](/assets/network-diagram.png)
Every Network diagram will have three zones they are

1. Trust/Internal Zone
2. DMZ/DMG (Demilitarized)
3. Internet/Public/External/Untrust

Critical servers will be deployed under trusted/internal zone. Couple of critical servers are:

1. Active Direct
2. Domain Controller (do the authentication and authorization part)
3. SMTP Server(for sending and addressing the emails)
4. DNS (Domain Name Resolution)
5. DHCP (Assigning the Ip address automatically)
6. WEB Server (for web applications, used to deploy organization related internal applications)
7. Data Base Server
8. SIEM tool (SERVER LAN)
9. EDR (SERVER LAN)

**Trust/Internal Zone**

Lets say the ip address range is 10.10.0/16 which is 2\*\*16 = 65535 ip addresses can be assigned for these servers.

### Infrastructure security/Vulnerability Management

For server side we perform scanning mechanism for secure related control by scanning the servers and identifying vulnerabilities known as **vulnerability assessment**. Managing and fixing of those vulnerabilities known as **vulnerability management** which falls under infrastructure security.

For every month we will do vulnerability assessment and management to fix we need to contact asset owner or server owner next raising the tickets by assigning to the asset owners which will be fixed by them.

Scanning should be done only on developing or testing environment. All these comes under server LAN.

**DMZ/DMG**
It act as a boundary between trust zone and untrust zone.

After scanning in developing and testing environment we will use tools like nessus which generates results automatically, then we have to do the manual vulnerability analysis then we have the report our asset support team/ business support team/ patch management team Then they will complete patch updates then we have the recheck with the patch update whether the vulnerabilities are really fixed are not.

##### Internet

It is a global network that connects billions of computer devices and mobiles by exchanging information. Which gives access for surfing internet, mails, social media.

But here starts the game where hackers attack on innocent people online through phishing emails, malicious websites.

### Networking Devices

These 5 devices will taken care by network administrator/engineers they perform configuration implement, trouble shooting,
managing and maintaining like any upgrade in the routers or switches.

##### Router

Router is a network connector or protocol convertor which is used to connect two different networks, it works on network layer (used for checking ip address) in OSI layer.

Example: When you access www.google.com, your request is broken into packets. These packets don’t travel directly to Google’s server-they pass through a series of routers that examine and forward them along the most efficient path until they reach the destination.

##### Switch

###### Access Switch

###### Distributed Switch

###### Core Switch

##### Load balancer (LB)

Balancing the load

NOC: Noc team functionality is monitoring and fixing the network or application or server issues 24*7*365 days. NOC monitoring tools are:

1. Solarwinds(compromised due to supply chain attack).
2. Netscope
3. Riverbed
4. Fluke Networks
5. What's up gold
6. PRTL
7. Datadog (in cloud environment)

### Network security Domains/Solution or Perimeter Solutions

If one layer (NGFW) is bypassing the attacks, second layer will prevent or block, in case second layer (Proxy) is bypassing then third layer (NIDS/NIPS) and so on. This layering is called as **Defense Depth Layer Approach**.

##### Firewall

Firewall is a system that prevents unauthorized access like ip's, ports entering into the private network. It creates safety barrier between private network and public network.

It is especially useful for large organization where hackers try to attack trough internet where this firewall tries to protect the network devices with in the organization. Let's say fires catches a house which has firewall that prevents fire passing through the wall so the rest of the house is safe.

Firewall rules plays curious role here where organizations set their rules which differ from each company. Let's take a example.

| Permission | IP Address | Protocol | Destination | Port |
| ---------- | ---------- | -------- | ----------- | ---- |
| Allow      | Any        | TCP      | Any         | 80   |
| Allow      | Any        | TCP      | Any         | 25   |
| Allow      | Any        | TCP      | Any         | 110  |
| Deny       | Any        | TCP      | Any         | 23   |
| Deny       | Any        | TCP      | Any         | 3389 |

This a firewall rule set table where we can see permission depends on ports in this table, in some companies they might have specific ip addresses and destinations as well, so ports from 80, 25 and 110 are allowed by the firewall and 23, 3389 are denied by the firewall.

Protocol TCP will be discussed further.

###### Types of Firewalls

1. Host Based Firewall
   It protects a individual computer where the software firewall has been installed.

2. Network Based Firewall
   It is combination of both hardware and software firewall where it protects entire network.

Types in network based firewall:

1. Stand-alone Firewall: Which is used by large organizations.
2. Built-in Firewall: Router have a built-in firewall which is lot of smaller organization relay on.
3. Cloud Firewall: Server providers firewall.

A lot of organizations use both network based and host based firewalls where network based protects whole network used by the organization and host based protects each systems used in the organization. If a bug passes through network firewall it can be prevented by host based firewall.

Analyst tasks: Check firewall logs for blocked vs. allowed traffic, unusual ports, or brute-force attempts.

##### VPN

Firewall fall under VPN itself we can also user separate VPN.

##### NIDS/NIPS

##### Proxy

##### End User LAN

End point/Host machines: Employee using an asset is called as end point. Example points are laptop,macbook, workstation, and mobile.

### End Point Security Solutions

AV/EDR/XDR - Malware prevention
DLP
HIDS/HIPS
FIM
Data at rest encryption
Mobile device management (MDM)

##### Email security solutions or email gateway

We have to deploy under the DMZ/DMG zone.

### Application Security / Product / IoT / OT / IIOT

WAF (Web Application firewall)
SDDLC
Criptography
owasp top 10

##### Internet Service Provider Router (ISP)

Anti DOS/Anti DDOS it will have monitoring tools if any flooding attacks are done by, our attacker either block or quarantining of those attacks.

##### Internet

Public network were we get internet.

each and every internal stack holder like HR Team, Application developing team and SOC team all the employees will fall under end use LAN segmentation part.
