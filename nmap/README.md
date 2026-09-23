# Nmap – Network Scanning Lab

## Overview

This lab covers the basic use of **Nmap (Network Mapper)** for network discovery and security assessment. Nmap is a free and open-source tool used to discover hosts, identify open ports, detect services and versions, and perform basic network reconnaissance.

The lab includes different Nmap scan types and a small real-world security assessment example.

## Objectives

- Understand what Nmap is and how it is used.
- Perform host discovery.
- Identify open and available ports.
- Understand different TCP and UDP scanning methods.
- Detect running services and their versions.
- Perform basic operating system detection.
- Understand how Nmap can be used for network inventory and security assessment.

## Tools Used

- **Nmap**
- **Kali Linux**
- **VirtualBox**

---

## 1. Basic Scan

### Command

```bash
nmap <Target-IP>
```

A basic Nmap scan checks commonly used TCP ports on the target and reports their state.

### Screenshot

![Basic Scan 1](screenshots/1-basic-scan-1.png)

![Basic Scan 2](screenshots/1-basic-scan-2.png)

---

## 2. Ping Scan (Host Discovery)

### Command

```bash
nmap -sn <Target-IP>
```

The `-sn` option performs host discovery without performing a port scan. It can be used to identify whether hosts are reachable on a network.

### Screenshot

![Ping Scan](screenshots/2-ping-host-discovery.png)

---

## 3. TCP SYN Scan

### Command

```bash
nmap -sS <Target-IP>
```

The `-sS` option performs a TCP SYN scan. It is commonly used to identify open TCP ports without completing the full TCP connection.

### Screenshot

![TCP SYN Scan](screenshots/3-tcp-syn-scan.png)

---

## 4. TCP Connect Scan

### Command

```bash
nmap -sT <Target-IP>
```

The `-sT` option performs a TCP connect scan. It establishes a complete TCP connection with the target port.

### Screenshot

![TCP Connect Scan](screenshots/4-tcp-connect-scan.png)

---

## 5. UDP Scan

### Command

```bash
sudo nmap -sU <Target-IP>
```

The `-sU` option is used to scan UDP ports. UDP services can include DNS, DHCP, SNMP, TFTP, and NTP.

### Screenshot

![UDP Scan](screenshots/5-udp-scan.png)

---

## 6. Service and Version Detection

### Command

```bash
nmap -sV <Target-IP>
```

The `-sV` option attempts to identify the services running on open ports and determine their versions.

### Screenshot

![Service Version Detection](screenshots/6-service-version-detection.png)

---

## 7. Operating System Detection

### Command

```bash
sudo nmap -O <Target-IP>
```

The `-O` option attempts to identify the operating system of the target based on network responses.

### Screenshot

![OS Detection](screenshots/7-os-detection.png)

---

## 8. Aggressive Scan

### Command

```bash
sudo nmap -A <Target-IP>
```

The `-A` option enables several advanced detection features, including operating system detection, service/version detection, default NSE scripts, and traceroute.

### Screenshot

![Aggressive Scan](screenshots/8-aggressive-scan.png)

---

## 9. Port Scan

### Command

```bash
nmap -p <Port Number> <Target-IP>
```

Specific ports can be selected for scanning.

For example:

```bash
nmap -p 22,80,443 <Target-IP>
```

A range of ports can also be specified:

```bash
nmap -p 20-100 <Target-IP>
```

### Screenshot

![Port Scan](screenshots/9-port-scan.png)

---

## 10. Scan All 65535 TCP Ports

### Command

```bash
nmap -p- <Target-IP>
```

The `-p-` option scans all 65,535 TCP ports instead of only the commonly used ports.

### Screenshot

![All TCP Ports](screenshots/10-all-65535-ports.png)

---

# Real-World Security Assessment Example

Consider a company that has expanded its office network and added new computers, servers, printers, IP phones, and other network devices.

A security team can use Nmap to:

1. Discover active devices on the network.
2. Identify open ports.
3. Detect running services and their versions.
4. Check for outdated services.
5. Compare identified software with known security advisories.
6. Disable unnecessary services and close unused ports.
7. Maintain an updated network asset inventory.
8. Identify potentially unauthorized devices.

This helps the security team understand the network and reduce unnecessary exposure.

## What I Learned

Through this lab, I learned how Nmap can be used for network reconnaissance and security assessment. I practiced host discovery, TCP and UDP scanning, service/version detection, OS detection, specific port scanning, and scanning all TCP ports.

I also understood how Nmap can help security teams maintain network visibility and identify potentially unnecessary or unauthorized services.

## Ethical and Legal Note

These scans should only be performed on systems and networks that you own or have explicit permission to assess. Unauthorized scanning of third-party systems can violate organizational policies or applicable laws.