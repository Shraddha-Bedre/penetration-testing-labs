# Penetration Testing Labs

## Overview

This repository contains my hands-on cybersecurity learning labs related to **network scanning, penetration testing, denial-of-service attack simulation, OWASP security testing, and web application security**.

These labs were completed as part of my cybersecurity learning and practical training. Each lab includes documentation and supporting screenshots where applicable.

---

## Labs Covered

### 1. Nmap

The Nmap lab covers different network scanning and host discovery techniques.

Topics include:

- Basic scanning
- Ping host discovery
- TCP SYN scanning
- TCP Connect scanning
- UDP scanning
- Service and version detection
- Operating system detection
- Aggressive scanning
- Port scanning
- Scanning all 65,535 ports

📁 **Folder:** `nmap`

---

### 2. DoS Attack Simulation

This lab demonstrates a controlled **SYN flood / DoS attack simulation** in a virtual lab environment.

The activity includes network configuration, connectivity testing, IIS setup, traffic generation, and packet analysis using Wireshark.

Topics include:

- Host-Only network configuration
- Static IP configuration
- Network connectivity verification
- IIS setup
- Wireshark packet capture
- SYN flood traffic analysis
- Wireshark display filters
- I/O Graph analysis
- Protocol Hierarchy
- Netstat analysis
- Windows Event Viewer

📁 **Folder:** `dos-attack-simulation`

---

### 3. OWASP & Penetration Testing

This lab covers the fundamentals of **OWASP and penetration testing**.

Topics include:

- OWASP overview
- OWASP projects and resources
- Penetration testing fundamentals
- Black Box, White Box, and Grey Box testing
- Phases of penetration testing
- Roles and responsibilities of a penetration tester
- OWASP Top 10
- OWASP Top 10 version comparison
- Using OWASP Top 10 during penetration testing
- Legal and ethical considerations

📁 **Folder:** `owasp-penetration-testing`

---

### 4. OWASP Juice Shop – Injection Challenges

This lab contains practical exercises performed using the intentionally vulnerable **OWASP Juice Shop** training application.

The challenges covered SQL Injection and NoSQL Injection concepts.

Topics include:

- Admin login challenge
- Login challenges
- Database schema
- User credential exposure
- Ephemeral Accountant
- NoSQL manipulation
- NoSQL exfiltration
- Completed challenge verification

📁 **Folder:** `owasp-juice-shop-injection`

---

## Tools & Technologies

The labs in this repository use a combination of cybersecurity and networking tools, including:

- Nmap
- Wireshark
- hping3
- OWASP Juice Shop
- Linux
- Windows
- VirtualBox
- IIS
- Networking concepts
- Web application security concepts

---

## Skills Demonstrated

Through these labs, I practiced:

- Network reconnaissance
- Port and service scanning
- Network traffic analysis
- Packet analysis
- Vulnerability identification
- Web application security testing
- SQL Injection concepts
- NoSQL Injection concepts
- Security assessment methodology
- Basic penetration testing techniques
- Security documentation and reporting
- Linux and Windows security fundamentals

---

## Repository Structure

```text
penetration-testing-labs
│
├── README.md
│
├── nmap
│   ├── README.md
│   └── screenshots
│
├── dos-attack-simulation
│   ├── README.md
│   └── screenshots
│
├── owasp-penetration-testing
│   └── README.md
│
└── owasp-juice-shop-injection
    ├── README.md
    └── screenshots
```

---

## What I Learned

These labs helped me gain practical understanding of:

- Network scanning and enumeration
- Identifying open ports and services
- Capturing and analyzing network traffic
- Understanding attack traffic patterns
- Using OWASP resources for application security
- Understanding common web application vulnerabilities
- Performing security testing in controlled environments
- Documenting security findings and observations
- Following ethical and authorized testing practices

---

## Ethical & Legal Notice

All activities documented in this repository were performed for **educational purposes in controlled and authorized lab environments**.

Security testing, scanning, traffic generation, and vulnerability exploitation should only be performed on systems, applications, networks, and devices for which explicit authorization has been obtained.

Do not use these techniques against systems or applications without permission.