## Computer Networking

## 📚 Table of Contents

- [ What is computer networking](#what-is-computer-networking)
- [Network Security Fundamentals](#network-security-fundamentals)
- [Types of Computer Networks](#types-of-computer-networks)

  - [LAN](#lan-local-area-network)
  - [WAN](#wan-wide-area-network)
  - [MAN](#man-metropolitan-area-network)

- [Network Monitoring and Security](#network-monitoring-and-security)

  - [Log](#log)
  - [SIEM](#siem-security-information-and-event-management)
  - [SOC](#soc-security-operation-center)
  - [DC - Data Center](#dc-data-center-on-premise)
  - [DC - Domain Controller](#dc-domain-controller)
  - [Authentication](#authentication)
  - [Authorization](#authorization)
  - [CIA](#cia-confidentiality-integrity-availability)

- [Ports and Protocols](#ports-and-protocols)

### What is computer networking?

Computer networking is known for communication between computer devices (computer, printers) by exchanging information between them.

It works both wired and wireless methods through wired mode like ethernet cables and wireless like bluetooth, wi-fi or nearby sharing.

---

### Types of Computer Networks

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

## Note: LAN is a subset of MAN.

---

### Network Monitoring and Security

### Log

Computer recorded activity.

![Log Event Viewer Diagram](/assets/log.png)

If you search for **event viewer** on your laptop you can see all logs that will be running in the backend right from the laptop switched on. Event ID **4624** is for user login successfully on the laptop which records each and every that user performed on his laptop.

Example: Windows laptop logs

Application, Audit or Security, System, Config

All the above logs will be integrated to SIEM tool using different log integration methods.

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

### Network Security Fundamentals

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

Messaging: SMTP - Simple Mail Transfer Protocol (25) used for sending and receiving messages, Pop 3 - Post Office Protocol (110) used for downloading messages to local folder, IMAP - Internet Message Access Protocol (143) used to for retrieving emails from a mail server, ICMP - Internet Control Message Protocol,
Terminal: SSH - Secure Shell (22), RDP - Remote Desktop Protocol (3389)

File Transfer:: FTP - File Transfer Protocol (20,21), SFTP - Secure File Transfer Protocol (22), NFS - Network File Sharing

DNS - Domain Name System (53), DHCP - Domain Host Configure Protocol (67,68),

### 6 Presentation Layer

Process of converting one form data into another.

[Encryption](#encryption),[Decryption](#decryption)

[Compression](#compression),[Decompression](#decompression)

[Encoding](#encoding), [Decoding](#decoding)

### 5 Session Layer

Managing the session between client and server.

Session Management

[Authentication](#authentication)

[Authorization](#authorization)

### 4 Transport Layer

Here the data will be transferred from source ip to destination ip with error flow control and data flow. Here data will be transferred in the form of [segments](#segmentation).

**Segmentation**

Dividing large chunk of data into small chunks.

**Error Flow Control**

Transferring data in a sequence order with our error.

**Data Flow Control**

Controls the speed of transferring data.

**TCP 3 way handshake**
This the process of communication between client and server where first client send sync flag to the server and server acknowledges and send sync+ack flag back to the server, next client after receiving sends back ack flag to the server for sending the request.

**TCP 2 way handshake**
This process is for connection closure first client sends the finish flag where server responds with acknowledgement flag.

| TCP                                                   | UDP                                                  |
| ----------------------------------------------------- | ---------------------------------------------------- |
| Transmission Control protocol                         | User Datagram Protocol                               |
| It is connection oriented                             | It is not based on connection oriented               |
| Data is transmitted as brocken packets called segment | Transmitted as datagram                              |
| Error Checking                                        | No error checking                                    |
| TCP is slower due to error check and flow control     | UDP is faster due to no error checking               |
| This will fall under Trasport Layer or layer 4        | This will also fall under Transport Layer or Layer 4 |

### 3. Network Layer

It provided end-to-end communication between two devices for source and destination using path determination by using ip address. Here **IP packets** are for data transfer through network.

**IP Packets**: consists of header(source and destination ip), payload(actual message or data).

**Path determination**: Choosing best path for data transfer.
Data will be transferred through ip address or logical address.

**Routing Protocols:**

1. Static route: data will be transferred in a fixed path.
2. Dynamic Route: based on routing traffic path is changed while transferring data.
3. Multi caste routing: Consists of multiple path for transferring data.
4. RIP (Routing Information Protocol): It is old method of dynamic router for data transfer through computers to choose best routing path.

### 2. Data Link Layers

It transfers data from source to destination in the form of frames.

##### Frames

It is type of data that consists of header, payload and trailer. Here the data is transferred in a local network LAN(ethernet cables).

**Header**
Consists of MAC address of source and destination devices.

Example: Data is transferring from computer to print where both MAC address will be stores in the header.

**Payload**

Stores IP packets which contains source and destination ip address from the upper-layer data, ip packets is actually used in [Network Layer](#3-network-layer).

### 1. Physical Layer

It provides end to end connection between two devices through physical medium. Example: LAN cable, ethernet. Here data is transferred through **bits**.

---

### Network Diagram

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

#### Infrastructure security/Vulnerability Management

For server side we perform scanning mechanism for secure related control by scanning the servers and identifying vulnerabilities known as **vulnerability assessment**. Managing and fixing of those vulnerabilities known as **vulnerability management** which falls under infrastructure security.

For every month we will do vulnerability assessment and management to fix we need to contact asset owner or server owner next raising the tickets by assigning to the asset owners which will be fixed by them.

Scanning should be done only on developing or testing environment. All these comes under server LAN.

**DMZ/DMG**
It act as a boundary between trust zone and untrust zone.

After scanning in developing and testing environment we will use tools like nessus which generates results automatically, then we have to do the manual vulnerability analysis then we have the report our asset support team/ business support team/ patch management team Then they will complete patch updates then we have the recheck with the patch update whether the vulnerabilities are really fixed are not.

#### Internet

It is a global network that connects billions of computer devices and mobiles by exchanging information. Which gives access for surfing internet, mails, social media.

But here starts the game where hackers attack on innocent people online through phishing emails, malicious websites.

#### Networking Devices

These 5 devices will taken care by network administrator/engineers they perform configuration implement, trouble shooting,
managing and maintaining like any upgrade in the routers or switches.

#### Router

Router is a network connector or protocol convertor which is used to connect two different networks, it works on network layer (used for checking ip address) in OSI layer.

Example: When you access www.google.com, your request is broken into packets. These packets don’t travel directly to Google’s server-they pass through a series of routers that examine and forward them along the most efficient path until they reach the destination.

#### Switch

It is a network device that connects multiple computer devices within a small area of network through LAN.

Types of switches

**Access Switch**: It is the first point of network connection to the end user and network. Just like connecting computer devices with lan ports or cables to the switches.

**Distributed Switch**: Aggregates all the access switch's and provide policy-based connectivity. Which filters the traffic, load balancing.

**Core Switch**: It connects to all the distributed switches and provide high-speed data transfer through out the whole organization. It provides high speed data transfer between distributed switches, data centers and servers which is more reliable.

#### Load balancer (LB)

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

If one layer (NGFW) is bypassing the attacks, second layer will prevent or block, in case second layer (Proxy) is bypassing then third layer (NIDS/NIPS) and so on. This layering is called as **Defense Depth Layer Approach** or **Onion Layer approach** just like onions there will be multiple layers of protection for data to prevent attacks.

##### NIDS/NIPS (Network Intrusion Detection/ Prevention System)

**NIDS** will watch and report which means it monitors the network traffic for any suspicious activity it alerts the administrator.

**NIPS** will prevent like blocking the traffic if there is any suspicious activity.

##### Proxy

Used to proxy IP address which gives **fake ip address** by hiding the original ip address.

##### End User LAN

End point/Host machines: Employee using an asset is called as end point. Example points are laptop,macbook, workstation, and mobile.

### End Point Security Solutions

AV/EDR/XDR - Malware prevention
DLP
HIDS/HIPS
FIM
Data at rest encryption
Mobile device management (MDM)

#### Firewall

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

**Types of Firewalls**

1. Host Based Firewall
   It protects a individual computer where the software firewall has been installed.

2. Network Based Firewall
   It is combination of both hardware and software firewall where it protects entire network.

**Types in network based firewall:**

1. Stand-alone Firewall: Which is used by large organizations.
2. Built-in Firewall: Router have a built-in firewall which is lot of smaller organization relay on.
3. Cloud Firewall: Server providers firewall.

A lot of organizations use both network based and host based firewalls where network based protects whole network used by the organization and host based protects each systems used in the organization. If a bug passes through network firewall it can be prevented by host based firewall.

Analyst tasks: Check firewall logs for blocked vs. allowed traffic, unusual ports, or brute-force attempts.

#### VPN

Firewall fall under VPN itself we can also user separate VPN.

#### Email security solutions or email gateway

We have to deploy under the DMZ/DMG zone.

### Application Security / Product / IoT / OT / IIOT

WAF (Web Application firewall)
SDDLC
Criptography
owasp top 10

#### Internet Service Provider Router (ISP)

Anti DOS/Anti DDOS it will have monitoring tools if any flooding attacks are done by, our attacker either block or quarantining of those attacks.

#### Internet

Public network were we get internet. Each and every internal stack holder like HR Team, Application developing team and SOC team all the employees will fall under end use LAN segmentation part.

### DHCP (Dynamic Host Configure Protocol)

When users computer connected to a network dhcp assigns a ip address automatically. Assigning ip to the system within a lease time where after completing the lease time the ip will be changing or we the system connects to new network it changes.

![DHCP Diagram](/assets/dhcp.png)

Here the network between system and router will be private address and the address between router and Internet will be public address.

**Static IP**: Fixed ip is used for communication. Assigning static ip for huge number of systems in a organization is difficult and time taking process as well. There will be ip conflicts as well due to multiple systems using same ip.

**Dynamic IP**: Changes ip address based on lease time.

### DORA (Discover Offer Request Acknowledgement)

Below steps are followed to get ip address assigned to a system.

1. First sends the **discover** message to the server saying system does'nt have any ip address to connect internet.
2. From the server it sends a **offer** message with list of available ip's that the system can acquire.
3. Then host sends a **request** message to acquire specific ip from the given list.
4. At last DHCP server sends a **acknowledge** message to the host saying host can use the ip addressed asked for.

If there is no availability of IP V4 then server provides IP V6 to the host.

### DNS (Domain Name System)

It is used to convert / resolve the domain name into ip address.

As a user we search for a domain name (netflix.com) but for the communication only binary code will be understood by the system. Where DNS helps to resolve the domain name into ip address.

First if we try to search a domain our browser will check that domain in the local browser cache if its available then it will directly redirect to that domain if it not available then it will be request to DNS resolver as **recursive query** for the ip address from the DNS server where there are 3 parts in DNS server they are:

**Root Server:** So after request if root server have ip address for that domain it will redirect to the domain directly else it will suggest to ask for TLD Server which is the 2nd part.

**TLD Server (Top Level Domains):** Here there be all world top level domains around 13 like .gov, .mil, .edu ..etc. If the ip address is available same it redirects else it forwards to the 3rd part which is authentative server.

**Authentative Server:** It is a ip pool where almost every ip address that are missing from the above two parts will be found here after redirecting to the ip address browser will stores the ip in cache. If the ip address is not found here as well then this means the domain is not registered.

---

### DNS Records

There are few DNS protocols to assign domain name to ip address or vise-versa.

| Record Name                  | Purpose                                                                              |
| ---------------------------- | ------------------------------------------------------------------------------------ |
| A                            | Assigning domain name to IP V4.                                                      |
| AAAA (Quad Record)           | Assigning or converting domain name to IP V6.                                        |
| MX (Mail Exchanger)          | Sending and receiving email through the server.                                      |
| CNAME (Canonical Name)       | Providing alias name for the domain name.                                            |
| TXT (Text Record)            | Storing the information of SPF, DMA, DMARC (found in gmail) for domain verification. |
| SOA (Start Of Authority)     | Storing the information of domain administrators.                                    |
| PTR (Pointer Reverse Record) | Converting IP Address to domain name which is also known as DNS reverse.             |

### IP Address (Internet Protocol)

IP address is for a system to communicate with servers or other systems, where ip address will be assigned once it is connected to internet. IP address is a **unique identifier** of a system.

**IP V4:** The size of the ip address V4 is 32 bits where the available addresses would be $2^{32}$ which is almost 4 billion. Format would be decimal with 4 octets(1 oct = 8 bites which is 4\*oct = 32 bits) separated by (.) with 8 bits each.

Example format: 192.168.0.1

**IP V6:**The size of the ip address V6 is 128 bits where the available addresses would be $2^{128}$ which is almost more than a trillion. Format would be with 16 octets(1 oct = 8 bites which is 16\*oct = 128 bits) separated by (:) with 8 bits each.

Example Format: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

There are two types of ip addresses:

1. Static IP Address: It is fixed ip address assigned manually for each system.
2. Dynamic IP Address: Changes dynamically based on lease time with the help of [DHCP](#dhcp-dynamic-host-configure-protocol).

To detect threat is from public or private address by the SOC analyst there few classes in both public and private IP's.

**Public IP Address:**

| Classes | Starting IP Address | Ending IP Address | Use case            |
| ------- | ------------------- | ----------------- | ------------------- |
| Class A | 0.0.0.0             | 126.255.255.255   | Large MNC's         |
| Class B | 128.0.0.0           | 191.255.255.255   | Mid range companies |
| Class C | 192.0.0.0           | 223.255.255.255   | Small companies     |
| Class D | 224.0.0.0           | 239.255.255.255   | Gaming              |
| Class E | 240.0.0.0           | 255.255.255.255   | Researching         |

For loop backup offline downloading **127.0.0.1** is used. You need too purchase public ip's from IANA (Internet Assign Numbering Authority).

IP Ranges formula:

from class B 128/2 + 128 = **64** + 128 = 192 (starting of class C) - 1 (ending of class B)

from class C **64/2** + 192 = **32** + 192 = 224 (starting of class D) - 1 (ending of class C)

from class D **32/2** + 224 = **16** + 224 = 240 (starting of class E) - 1 (ending of class E)

**Private IP Address:**

| Classes | Starting IP Address | Ending IP Address |
| ------- | ------------------- | ----------------- |
| Class A | 10.0.0.0            | 10.255.255.255    |
| Class B | 172.16.0.0          | 172.31.255.255    |
| Class C | 192.68.0.0          | 192.68.255.255    |

**Subnet Masking**

Subnet masking is used to divide large network into small network chunks.

| CIDR - Classless Inter Domain Routing | Subnet Mask     |
| ------------------------------------- | --------------- |
| /8                                    | 255.0.0.0       |
| /16                                   | 255.255.0.0     |
| /24                                   | 255.255.255.0   |
| /30                                   | 255.255.255.252 |

### MAC Address

MAC address is a unique identifier for a physical data transferring devices which will be assigned at the manufacturing level itself. It will be 48 bits of size so $2^{48}$ addresses are available. MAC address will be in the format of hexadecimal which is alphanumeric and it has 8 octants separated by colons(:).Example format: 00:1A:2B:3C:4D:5E

Example: Router, LAN cable ...etc.

---

### Ports And Protocols

### Protocols

It is **set of rules** used for communication between devices over a network for smooth data transmitting and receiving.

Example: HTTPS -> Web browsing, SMTP -> Mailing, FTP -> File Sharing ...etc.

### Ports

Ports is a **logical end point** used for application to identify the process or which type of network service.

IP Address is for identifying the device for network communication. It's like a town or village name.

Port is for identifying which application to receive network or data in a system. It's like a house number.

Total there 65,535 ports and divided into 3 parts.

| Port Ranges   | Type                           | Description                               |
| ------------- | ------------------------------ | ----------------------------------------- |
| 0 - 1023      | Well known ports/ System ports | Network services like HTTPS, FTP, SMTP    |
| 1024 - 49151  | Registered Ports               | For custom apps like My Sql.              |
| 49152 - 65534 | Private Ports                  | Used For client communication temporarily |

There are two types of ports:

**Open port:** Here network actively accepts traffic which is not safe any cost.

**Closed Port:** It is safe for data transmitting and receiving.

**Commonly Used ports and protocols**

| Protocols                                   | Description                                                                                              | Ports                    |
| ------------------------------------------- | -------------------------------------------------------------------------------------------------------- | ------------------------ |
| HTTP (Hyper Text Transfer Protocol)         | Used for web-browsing which is not secure.                                                               | 80                       |
| HTTPS (Hyper Text Transfer Protocol Secure) | Used for secure web-browsing.                                                                            | 443                      |
| FTP (File Transfer Protocol)                | File transferring over a network not secured                                                             | 20, 21                   |
| SFTP (Secure File Transfer Protocol)        | Secure File transferring over a network                                                                  | 22                       |
| SMTP (Simple Mail Transfer Protocol)        | Sending and receiving mails over a network                                                               | 25                       |
| DNS (Domain Name Server)                    | Resolving domain name into ip address.                                                                   | 53                       |
| DHCP (Domain Host Configure Protocol)       | Dynamic assigning of ip address to a system.                                                             | 67 (server), 68 (client) |
| SSL (Secure Socket Layer)                   | Establishing secure connection between web browser and server                                            | 443                      |
| TLS (Transport Layer Security)              | Used for same SSL purpose by fixing SSL vulnerabilities                                                  | 443                      |
| NTP (Network Time Protocol)                 | Used to synchronize your tool time with the local time.                                                  | 123                      |
| SMB (Server Message Blocking)               | Used for file transferring an messaging over a network                                                   | 445                      |
| IMAP (Internet Message Access Protocol)     | Retrieving messages over a network                                                                       | 143                      |
| ICMP (Internet Control Message Protocol)    | Sending error messages to the source host if there is any attack or suspicious over a network connection | no port                  |
| POP3                                        | Used to download messages to the local folder                                                            | 110                      |
| SCP (Secure Copy Protocol)                  | Used transfer data over a network by using SSH encryption and authentication                             | 22                       |
| Telnet                                      | Remote login, not secured                                                                                | 23                       |
| SSH (Secure Shell)                          | Remote Login and command execution                                                                       | 22                       |
| RDP (Remote Desktop Protocol)               | Remote login through windows to windows                                                                  | 3389                     |
| Kerberos                                    | Mutual authentication for both client and server while transmitting files over a insecure network        | 88                       |
| MySql                                       | Database for storing and managing data.                                                                  | 3306                     |
