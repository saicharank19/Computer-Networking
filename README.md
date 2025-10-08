### Computer Networking

#### What is computer networking?

Computer networking is known for communication between computer devices (computer, printers) by exchanging information between them.

It works both wired and wireless methods through wired mode like ethernet cables and wireless like bluetooth, wi-fi or nearby sharing

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

