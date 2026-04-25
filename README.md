
# 🔐 SQL Injection Security Assessment & Exploitation Validation OWASP Bricks Login-1
---

## 📌 Overview
### This project presents a hands-on web application security assessment focused on identifying and validating SQL Injection (SQLi) vulnerabilities in a controlled and authorized environment of OWASP Bricks Login-1 Page The assessment demonstrates both **manual testing techniques** and **automated validation workflows**, showcasing practical cybersecurity skills relevant to penetration testing and application security.

---
## 🎯 Objectives

- Identify SQL Injection vulnerabilities in OWASP Bricks Login-1 form
- Validate findings using both manual and automated approaches
- Analyze HTTP requests and application responses
- Demonstrate exploitation in a controlled environment
- Produce a professional security report with remediation guidance

---

## 📍 Scope

- Target: Intentionally vulnerable web application
- Focus Area: Login functionality
- Testing Type:
  - Input validation testing
  - Authentication bypass attempts
  - Backend query behavior observation

---

## 🛠️ Tools & Environment

- 🐧 Kali Linux
- 🕷️ Burp Suite (Proxy & Request Interception)
- ⚙️ sqlmap (Automated SQL Injection Tool)
- 📄 SQL Injection Wordlists (Local Reference)
- 🌐 Web Browser

---

## 🔍 Methodology

### 1. Manual SQL Injection Testing

The assessment began with manual interaction with the login form:

- Submitted normal credentials to establish **baseline behavior**
- Injected SQL payloads from a reference wordlist
- Observed:
  - Authentication responses
  - Error messages
  - Application behavior changes

🔎 **Goal:** Identify improper input handling and query construction

---

### 2. HTTP Request Analysis (Burp Suite)

- Intercepted login requests using Burp Suite
- Analyzed:
  - HTTP POST parameters
  - Request structure
  - Server responses

📌 This step confirmed how user input was transmitted and processed.

---

### 3. Automated Validation (sqlmap)

- Exported captured request to sqlmap
- Used sqlmap to:
  - Confirm SQL injection vulnerability
  - Identify injectable parameters
  - Demonstrate potential database interaction (controlled)

---
## ⚠️ Key Findings
- The login form was vulnerable to SQL Injection

- User input was not properly sanitized or parameterized

- Authentication logic could be bypassed

- Backend database queries were exposed to manipulation

