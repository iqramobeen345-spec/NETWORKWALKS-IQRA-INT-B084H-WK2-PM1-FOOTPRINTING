# NETWORKWALKS-IQRA-INT-B084H-WK2-PM1-FOOTPRINTING
Week 2 Cybersecurity Internship Tasks – Practical Footprinting Exercises using GHDB, Maltego, and other OSINT tools.
# 🛡️ WEEK 2 – CYBERSECURITY & ETHICAL HACKING LAB

**Footprinting, Reconnaissance & Network Scanning**

A practical cybersecurity project completed as part of the NetworkWalks Cybersecurity Internship. This repository documents hands-on exercises using Kali Linux, Maltego, theHarvester, Zenmap and multiple reconnaissance tools.

---

## 📑 Table of Contents

1. Overview
2. Project at a Glance
3. Tools & Technologies
4. Project Modules
5. Module 1 – Footprinting with Multiple Kali Tools
6. Module 3 – Footprinting with Maltego
7. Module 4 – Footprinting with theHarvester
8. Module 5 – Network Scanning with Zenmap
9. Network Scanning Results
10. Screenshots & Documentation
11. Skills Demonstrated
12. Learning Outcomes
13. Ethical Considerations & Disclaimer
14. Author
15. References

---

## 🎯 Overview

This project focuses on practical cybersecurity techniques, including information gathering, footprinting, reconnaissance and network scanning.

The main objective was to understand how cybersecurity professionals collect publicly available information about domains, identify network devices, discover live hosts and analyze network infrastructure using different security tools.

The exercises were performed using Kali Linux and Windows-based security tools for educational purposes.

## 📊 Project at a Glance

| Component | Details |
|---|---|
| Internship | NetworkWalks Cybersecurity Internship |
| Week | Week 2 |
| Domain | Cybersecurity & Ethical Hacking |
| Operating System | Kali Linux & Windows |
| Reconnaissance Tools | WHOIS, WhatWeb, NSLookup, cURL, WAFW00F, DNSRecon |
| OSINT Tool | Maltego |
| Information Gathering | theHarvester |
| Network Scanning | Zenmap / Nmap |
| Network | Local LAN |
| Main Activities | Footprinting, OSINT, DNS Enumeration, Network Scanning |

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Penetration testing environment |
| WHOIS | Domain registration information |
| WhatWeb | Website technology fingerprinting |
| NSLookup | DNS lookup and IP resolution |
| cURL | HTTP response header analysis |
| WAFW00F | Web Application Firewall detection |
| DNSRecon | DNS record enumeration |
| Maltego | Visual information gathering and link analysis |
| theHarvester | Email and subdomain collection |
| Zenmap | Graphical network scanning |
| Nmap | Network discovery and scanning |
| Windows CMD | Local IP and network configuration |

---

## 🔍 Module 1 – Footprinting & Reconnaissance with Multiple Kali Tools (W2-PM1)

### Objective

To gather publicly available information about the target domain `networkwalks.com` using six built-in Kali Linux tools.

### Tasks Performed

**1. WHOIS – Domain Information**

Command:

```bash
whois networkwalks.com
```

Purpose:
- Identify domain registration details.
- Find registrar information.
- Examine name servers and registration dates.

**2. WhatWeb – Website Fingerprinting**

Command:

```bash
whatweb networkwalks.com
```

Purpose:
- Identify website technologies.
- Detect CMS and web server information.
- Examine publicly exposed technology details.

**3. NSLookup – DNS Resolution**

Command:

```bash
nslookup networkwalks.com
```

Purpose:
- Resolve domain names into IP addresses.
- Examine DNS responses.

**4. cURL – HTTP Header Analysis**

Command:

```bash
curl -I https://networkwalks.com
```

Purpose:
- Retrieve HTTP response headers.
- Examine server information and response status.
- Identify publicly exposed header information.

**5. WAFW00F – Firewall Detection**

Command:

```bash
wafw00f networkwalks.com
```

Purpose:
- Identify whether a Web Application Firewall is present.
- Understand the website's security protection layer.

**6. DNSRecon – DNS Enumeration**

Command:

```bash
dnsrecon -d networkwalks.com
```

Purpose:
- Enumerate DNS records.
- Identify name servers and mail servers.
- Examine TXT and other DNS records.

---

## 🕸️ Module 3 – Footprinting with Maltego (W2-PM3)

### Objective

To install and configure Maltego on Windows and collect publicly available email information associated with the authorized training domain.

### Tasks Performed

1. Downloaded Maltego from its official website.
2. Installed Maltego on Windows.
3. Completed application configuration.
4. Created a free Maltego account.
5. Logged into the application.
6. Created a new investigation graph.
7. Added a Domain entity.
8. Entered `networkwalks.com` as the target domain.
9. Selected email-related transforms.
10. Executed the transforms to identify associated email addresses.

### Tool Information

**Maltego:** An OSINT and link-analysis tool used to visualize relationships between domains, email addresses, organizations and other publicly available information.

Official Website: https://www.maltego.com/

---

## 📧 Module 4 – Footprinting & Reconnaissance with theHarvester (W2-PM4)

### Objective

To collect email addresses and subdomains associated with the target organization using theHarvester in Kali Linux.

Target domain: `microsoft.com`

### Task 1 – Search Using Baidu

Command:

```bash
theHarvester -d microsoft.com -l 1000 -b baidu
```

Purpose:
- Search public information using Baidu.
- Collect email addresses and subdomains.
- Limit the search results to 1000.

### Task 2 – Search Using All Sources

Command:

```bash
theHarvester -d microsoft.com -l 50 -b all
```

Purpose:
- Search using supported data sources.
- Gather publicly available email addresses and subdomains.
- Limit the results to 50.

### Documentation

For both tasks:
- Executed the commands in Kali Linux.
- Examined the collected information.
- Captured screenshots of the results.
- Saved command outputs in text files.

---

## 🌐 Module 5 – Network Scanning with Zenmap (W2-PM5)

### Objective

To identify live hosts, IP addresses and MAC addresses within the local network using Zenmap.

### Tasks Performed

**1. Download and Installation**

Downloaded and installed Zenmap on Windows using the official Nmap download page.

https://nmap.org/download.html

**2. Local IP Address Identification**

Used Windows Command Prompt:

```cmd
ipconfig
```

This command displays local network configuration, including IPv4 address and subnet information.

**3. Live Host Discovery**

Opened Zenmap and selected the Ping Scan profile to discover active hosts within the local subnet.

**4. Network Topology**

Viewed the network topology, enabled the topology legend and exported the graphical network representation in PDF format.

---

## 📊 Network Scanning Results

The following results were recorded in the Zenmap lab exercise.

**Live Hosts Identified:**

4 hosts, including the local PC.

**IP Addresses:**

| No. | IP Address |
|---|---|
| 1 | 10.0.0.1 |
| 2 | 10.0.0.4 |
| 3 | 10.0.0.19 |
| 4 | 10.0.0.5 |

**MAC Addresses:**

| No. | MAC Address |
|---|---|
| 1 | 00:50:56:E3:B3:2C |
| 2 | 00:0C:29:C0:94:8F |
| 3 | 00:50:56:E9:64:82 |
| 4 | 00-0C-29-40-C0-93 |

*Note: These are the recorded lab results. Network addresses and discovered devices may vary depending on the network environment.*

---

## 📸 Screenshots & Documentation

Screenshots and supporting documentation are organized in the repository's `screenshots` folder.

The screenshots document:

- Kali Linux reconnaissance commands and outputs.
- WHOIS and DNS enumeration.
- Website fingerprinting and HTTP header analysis.
- Maltego installation and investigation graph.
- theHarvester search results.
- Zenmap installation and network scanning.
- Live host discovery and network topology.

The final penetration-testing report and Zenmap topology PDF can also be included in the repository as supporting documents.

---

## 💡 Skills Demonstrated

Through these practical exercises, the following skills were developed:

- Footprinting and reconnaissance.
- Open-Source Intelligence (OSINT).
- Domain and DNS information gathering.
- Website technology fingerprinting.
- HTTP response header analysis.
- Web Application Firewall identification.
- Email and subdomain enumeration.
- Network scanning and host discovery.
- IPv4 addressing and subnet identification.
- MAC address identification.
- Network topology visualization.
- Security documentation and reporting.
- Kali Linux command-line operations.

---

## 🎓 Learning Outcomes

This project provided practical experience in understanding the initial stages of ethical hacking and cybersecurity assessments.

Key learning outcomes:

1. Understood the importance of reconnaissance in penetration testing.
2. Learned to use multiple Kali Linux tools for information gathering.
3. Practiced visual OSINT investigations using Maltego.
4. Learned email and subdomain enumeration using theHarvester.
5. Identified live devices within a local network using Zenmap.
6. Improved understanding of IP addresses, MAC addresses and network topology.
7. Practiced documenting technical findings through screenshots and reports.

---

## ⚠️ Ethical Considerations & Disclaimer

This project is strictly intended for educational purposes and authorized cybersecurity testing.

All reconnaissance and scanning activities must be performed only on systems, networks and domains that you own or have explicit permission to assess.

Unauthorized access, scanning or misuse of collected information is prohibited.

The purpose of these exercises is to develop cybersecurity knowledge and improve defensive security awareness.

---

## 👩‍💻 Author

**Iqra Mobeen**

Cybersecurity & IT Student  
Cybersecurity B084  
NetworkWalks Cybersecurity Internship

**Areas of Interest:**
- Cybersecurity
- Ethical Hacking
- Network Security
- Network Reconnaissance
- Information Security

---

## 📚 References

- NetworkWalks Academy – Cybersecurity & Ethical Hacking Week 2 Project Modules.
- Maltego Official Website: https://www.maltego.com/
- Nmap Official Website: https://nmap.org/
- Kali Linux Official Website: https://www.kali.org/
- theHarvester GitHub Repository: https://github.com/laramies/theHarvester

---

**Thank you for exploring my Week 2 Cybersecurity Internship work!**
