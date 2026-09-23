# OWASP & Penetration Testing

## Overview

This lab covers the fundamentals of **OWASP (Open Worldwide Application Security Project)** and **Penetration Testing**. It focuses on understanding common web application security risks, the OWASP Top 10, penetration testing phases, and the legal and ethical responsibilities of an ethical hacker.

The topics covered in this lab are based on my cybersecurity coursework and practical learning.

---

## Objectives

- Understand the purpose and importance of OWASP.
- Learn the fundamentals of penetration testing.
- Understand the roles and responsibilities of a penetration tester.
- Study the OWASP Top 10 security risks.
- Compare OWASP Top 10 versions from 2017 and 2021.
- Understand how OWASP Top 10 can be used during penetration testing.
- Learn the legal and ethical responsibilities of ethical hackers.

---

## 1. What is OWASP?

**OWASP (Open Worldwide Application Security Project)** is a non-profit organization focused on improving the security of software and web applications.

OWASP provides free:

- Security tools
- Documentation
- Security standards
- Research
- Educational resources

One of the most well-known OWASP resources is the **OWASP Top 10**, which provides a list of important security risks affecting web applications.

### Important OWASP Projects

- OWASP Web Security Testing Guide (WSTG)
- OWASP Application Security Verification Standard (ASVS)
- OWASP Cheat Sheet Series
- OWASP Juice Shop
- OWASP ZAP (Zed Attack Proxy)

### Importance of OWASP

OWASP helps developers, security professionals, testers, and organizations understand common application security risks and apply appropriate security practices to protect applications and sensitive information.

---

## 2. Penetration Testing

**Penetration Testing**, also called **Pen Testing**, is a security testing process in which an ethical hacker simulates real-world cyberattacks to identify vulnerabilities in a system, network, web application, or other authorized target.

The main objectives are to:

- Identify security weaknesses.
- Understand the potential impact of vulnerabilities.
- Provide recommendations for fixing identified issues.
- Verify whether security controls are working effectively.

Penetration testing must always be performed with proper authorization and within an approved scope.

### Types of Penetration Testing

#### Black Box Testing

The tester has little or no prior knowledge about the target system. This is similar to an external attacker attempting to discover vulnerabilities.

#### White Box Testing

The tester has detailed information about the target, such as source code, architecture, and credentials.

#### Grey Box Testing

The tester has partial information about the target system. It combines aspects of both black-box and white-box testing.

### Phases of Penetration Testing

1. Planning and Scoping
2. Information Gathering
3. Vulnerability Scanning
4. Exploitation
5. Post-Exploitation
6. Reporting
7. Remediation Verification

### Roles and Responsibilities of a Penetration Tester

A penetration tester is responsible for:

- Obtaining proper authorization before testing.
- Understanding the approved scope.
- Gathering information about the target.
- Performing vulnerability assessments.
- Testing vulnerabilities in a controlled manner.
- Determining the potential impact of findings.
- Documenting findings and evidence.
- Providing appropriate risk information.
- Suggesting practical remediation steps.
- Maintaining confidentiality.
- Retesting vulnerabilities after remediation.
- Staying updated with security tools and techniques.

### Skills Required

A penetration tester should have knowledge of:

- Networking concepts
- Windows and Linux operating systems
- Web application security
- Programming and scripting
- Basic cryptography
- Security tools such as Nmap, Burp Suite, Metasploit, Wireshark, and OWASP ZAP
- Technical documentation and report writing

---

## 3. OWASP Top 10

The **OWASP Top 10** is a widely used awareness and reference document covering important security risks in web applications.

It helps developers and security professionals understand common application security weaknesses and consider appropriate security controls.

### OWASP Top 10 – 2025

The coursework for this lab covered the 2025 release-candidate topics as follows:

1. Broken Access Control
2. Cryptographic Failures
3. Injection
4. Insecure Design
5. Security Misconfiguration
6. Vulnerable and Outdated Components
7. Identification and Authentication Failures
8. Software and Data Integrity Failures
9. Security Logging and Monitoring Failures
10. Server-Side Request Forgery (SSRF)

### OWASP Top 10 – 2021

1. **A01:2021 – Broken Access Control**  
   Users can access data or perform actions beyond their permissions.

2. **A02:2021 – Cryptographic Failures**  
   Sensitive information may be exposed because encryption is missing or incorrectly implemented.

3. **A03:2021 – Injection**  
   Malicious input can be interpreted as commands or queries by an application.

4. **A04:2021 – Insecure Design**  
   Security weaknesses are introduced during application design.

5. **A05:2021 – Security Misconfiguration**  
   Incorrect or insecure configuration can expose an application to attacks.

6. **A06:2021 – Vulnerable and Outdated Components**  
   Applications may contain components with known security vulnerabilities.

7. **A07:2021 – Identification and Authentication Failures**  
   Weak authentication mechanisms can allow attackers to compromise accounts.

8. **A08:2021 – Software and Data Integrity Failures**  
   Applications may trust software, updates, or data without proper integrity verification.

9. **A09:2021 – Security Logging and Monitoring Failures**  
   Poor logging and monitoring can make attacks difficult to detect.

10. **A10:2021 – Server-Side Request Forgery (SSRF)**  
    A vulnerable server may be manipulated into making unintended requests to other systems.

### OWASP Top 10 – 2017

1. A1 – Injection
2. A2 – Broken Authentication
3. A3 – Sensitive Data Exposure
4. A4 – XML External Entities (XXE)
5. A5 – Broken Access Control
6. A6 – Security Misconfiguration
7. A7 – Cross-Site Scripting (XSS)
8. A8 – Insecure Deserialization
9. A9 – Using Components with Known Vulnerabilities
10. A10 – Insufficient Logging and Monitoring

### Comparison of OWASP Versions

The OWASP Top 10 has changed over time as application security risks and industry practices have evolved.

Some notable changes between the 2017 and 2021 versions include:

- **Sensitive Data Exposure** was replaced by **Cryptographic Failures**.
- **Broken Authentication** became **Identification and Authentication Failures**.
- **XXE** was incorporated into other categories.
- **XSS** became part of the broader **Injection** category.
- **Insecure Deserialization** was addressed through the broader **Software and Data Integrity Failures** category.
- **Using Components with Known Vulnerabilities** became **Vulnerable and Outdated Components**.
- **Insufficient Logging and Monitoring** became **Security Logging and Monitoring Failures**.

These changes reflect the evolving focus of application security.

---

## 4. OWASP Top 10 in Penetration Testing

The OWASP Top 10 can be used as a reference when performing web application security assessments.

Instead of testing randomly, a penetration tester can use the categories to organize the assessment and consider common vulnerability areas.

Examples include:

- **Broken Access Control:** Check whether users can access resources or functions outside their permissions.
- **Injection:** Test whether untrusted input is interpreted as commands or queries.
- **Authentication Failures:** Review authentication, password policies, and session management.
- **Security Misconfiguration:** Review application and server configurations.
- **Vulnerable Components:** Identify outdated software and components with known vulnerabilities.
- **Logging and Monitoring:** Check whether important security events are properly recorded and monitored.

### Benefits

- Provides a structured testing approach.
- Helps identify important application security risks.
- Improves consistency during security assessments.
- Reduces the chance of missing common vulnerability areas.
- Helps organizations prioritize remediation.
- Supports application security improvement.

---

## 5. Code of Conduct and Legal & Ethical Considerations

Penetration testing must always be performed responsibly and with proper authorization.

### Code of Conduct

#### 1. Obtain Proper Authorization

Written permission should be obtained before beginning security testing.

#### 2. Work Within the Approved Scope

Only systems, applications, networks, and activities included in the agreed scope should be tested.

#### 3. Maintain Confidentiality

Sensitive information discovered during testing must be protected and should not be shared with unauthorized individuals.

#### 4. Avoid Causing Damage

Testing should be performed carefully to avoid unnecessary disruption, data loss, or impact on business operations.

#### 5. Report Findings Honestly

Security findings should be documented accurately without hiding or exaggerating vulnerabilities.

#### 6. Protect Client Data

Credentials, collected information, evidence, and reports should be stored securely and handled according to the agreed requirements.

#### 7. Follow Professional Standards

A penetration tester should act professionally, respect privacy, and follow organizational policies.

### Legal Considerations

A penetration tester should:

- Obtain written permission before testing.
- Respect privacy and applicable data protection requirements.
- Avoid accessing systems outside the approved scope.
- Never intentionally steal, modify, or delete data.
- Follow contractual agreements such as NDAs.
- Follow organizational security policies.

Unauthorized security testing can have legal consequences even when the intention is to identify security weaknesses.

### Ethical Considerations

An ethical hacker should:

- Act honestly and responsibly.
- Respect user privacy.
- Keep sensitive information confidential.
- Never misuse discovered vulnerabilities.
- Avoid conflicts of interest.
- Report vulnerabilities responsibly.

---

## What I Learned

Through this lab, I learned:

- The purpose and importance of OWASP.
- The fundamentals and phases of penetration testing.
- Different types of penetration testing.
- Roles and responsibilities of a penetration tester.
- Common web application security risks covered by the OWASP Top 10.
- How OWASP Top 10 can be used as a reference during security assessments.
- The differences between OWASP Top 10 versions.
- The importance of authorization, scope, confidentiality, and responsible security testing.

---

## Conclusion

This lab helped me understand the fundamentals of **OWASP and penetration testing**. I learned how the OWASP Top 10 can be used as a reference for identifying common web application security risks and how penetration testers should conduct assessments in an authorized and controlled manner.

The lab also highlighted the importance of following legal, ethical, and professional practices while performing security testing.

---

## Ethical & Legal Notice

All security testing discussed in this lab is intended for **educational purposes and authorized environments only**.

Penetration testing should only be performed on systems, applications, networks, and devices for which explicit permission has been obtained.