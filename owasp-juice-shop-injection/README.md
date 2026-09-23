# OWASP Juice Shop – Injection Challenges

## Overview

This lab covers selected injection and related security challenges from **OWASP Juice Shop**, an intentionally vulnerable web application designed for security training and learning.

The exercises helped me understand how different types of injection vulnerabilities can affect web applications and how security testers can identify them in an authorized lab environment.

---

## Objectives

- Understand the purpose of OWASP Juice Shop.
- Learn about common injection vulnerabilities.
- Practice identifying SQL Injection and NoSQL Injection scenarios.
- Understand how insecure input handling can affect web applications.
- Observe the results of security testing in a controlled environment.
- Understand the importance of secure input validation and database queries.

---

## Lab Environment

| Component | Details |
|---|---|
| Application | OWASP Juice Shop |
| Purpose | Web Application Security Training |
| Testing Type | Authorized Security Testing |
| Main Topics | SQL Injection and NoSQL Injection |
| Testing Environment | Local / Controlled Lab |

---

## OWASP Juice Shop

**OWASP Juice Shop** is an intentionally insecure web application created for security education and penetration testing practice.

It contains different types of vulnerabilities commonly found in real-world web applications. These challenges can be used to understand application security concepts in a safe and controlled environment.

---

# Challenges Performed

## 1. Login Admin

This challenge demonstrates a **SQL Injection** vulnerability in the login functionality.

The application does not properly handle the user input used during authentication. By manipulating the input, the normal authentication logic can be affected.

**Screenshot:** `1-Login Admin`

---

## 2. Login as Jim and Bender

This challenge demonstrates how insecure authentication logic can be affected by SQL Injection.

The exercise was performed for the test accounts **Jim** and **Bender** in the Juice Shop lab environment.

**Screenshot:** `2-Successfully Login as Jim and Bender`

---

## 3. Database Schema

This challenge demonstrates how SQL Injection can be used to understand information about the application's database structure.

The testing involved observing database responses and identifying information related to the database schema.

**Screenshot:** `3-Database Schema`

---

## 4. User Credentials

This challenge demonstrates the security impact of SQL Injection when database information containing user credentials is exposed.

The exercise helped me understand why applications should properly validate user input and use secure database query methods.

**Screenshot:** `4-All user credentials`

---

## 5. Ephemeral Accountant

This challenge demonstrates another SQL Injection scenario in the Juice Shop application.

The exercise involved manipulating application input and observing how database queries responded to the modified input.

**Screenshot:** `5-Ephemeral Accountant`

---

## 6. NoSQL Manipulation

This challenge demonstrates a **NoSQL Injection** scenario.

The request was modified during testing to observe how the application handled manipulated input in the review functionality.

**Screenshot:** `6-After writing and editing review`

---

## 7. NoSQL Manipulation Result

After the NoSQL manipulation, the modified review content became visible across products in the lab application.

This demonstrated the possible impact of insufficient input validation and authorization checks when handling database operations.

**Screenshot:** `7-The Hacked! message appears in reviews for all products`

---

## 8. NoSQL Exfiltration

This challenge demonstrates a NoSQL Injection scenario involving the extraction of application data.

The exercise helped me understand how improperly handled database queries can potentially expose information that should not be accessible.

**Screenshot:** `8-Extracted Data`

---

## 9. NoSQL Exfiltration – Additional Result

The additional screenshot shows the extracted information obtained during the NoSQL Injection challenge.

**Screenshot:** `9-Extracted Data`

---

## 10. Completed Challenges

The final screenshot shows the completed Juice Shop challenges from this assignment.

**Screenshot:** `10-All completed challenges`

---

# Key Security Concepts Learned

### SQL Injection

SQL Injection occurs when untrusted user input is incorrectly included in database queries. An attacker may manipulate the query logic and potentially access or modify information.

### NoSQL Injection

NoSQL Injection occurs when applications incorrectly process user-controlled input in NoSQL database queries. Manipulated input may change the intended database operation.

### Input Validation

Applications should properly validate and sanitize user input before processing it.

### Secure Database Queries

Applications should use secure query techniques such as parameterized queries and appropriate database APIs instead of directly constructing queries from untrusted input.

### Authentication Security

Authentication functionality should be designed so that user input cannot bypass authentication checks.

---

# What I Learned

Through these Juice Shop challenges, I learned:

- How OWASP Juice Shop can be used for web security training.
- Basic concepts of SQL Injection.
- Basic concepts of NoSQL Injection.
- How insecure input handling can affect application functionality.
- How database-related vulnerabilities can expose sensitive information.
- The importance of input validation.
- The importance of secure database query practices.
- The importance of testing web applications in an authorized environment.

---

# Conclusion

This lab provided practical exposure to common injection vulnerabilities using the OWASP Juice Shop training application.

By completing these challenges, I gained a better understanding of how SQL and NoSQL injection vulnerabilities can affect authentication, database operations, application data, and other web application functionality.

The exercises also helped me understand why secure input handling, authentication controls, and secure database queries are important for protecting web applications.

---

## Ethical & Legal Notice

This lab was performed for **educational and cybersecurity learning purposes** using an intentionally vulnerable training application.

Security testing should only be performed on systems and applications where explicit authorization has been provided. The techniques learned from this lab should not be used against real systems, websites, accounts, or data without permission.