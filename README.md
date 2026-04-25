
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

---
## 🔥 Security Impact
- Unauthorized access to application accounts

- Potential database enumeration

- Risk of sensitive data exposure

- Compromise of application integrity

---
## 🛡️ Recommendations

To mitigate SQL Injection vulnerabilities:

- ✅ Use Prepared Statements / Parameterized Queries
  
- ✅ Implement Input Validation & Sanitization

- ✅ Apply Web Application Firewall (WAF)

- ✅ Enforce Least Privilege Database Access

- ✅ Improve Error Handling (avoid detailed DB errors)

---
## 📚 Skills Demonstrated
- Web Application Security Testing

- SQL Injection Exploitation Techniques

- HTTP Request Analysis

- Use of Burp Suite & sqlmap

- Vulnerability Reporting & Documentation

- Secure Coding Awareness

---
## 📈 Conclusion

This project highlights how insecure input handling can lead to critical vulnerabilities such as SQL Injection. By combining manual testing with automated tools, the assessment provides a comprehensive understanding of both the discovery and validation process.

The exercise reinforces the importance of secure development practices and demonstrates practical, job-ready cybersecurity skills.

---
### ⚠️ Note: This project was conducted on an intentionally vulnerable training application for educational and portfolio purposes only.

---
## 👤 Author

Adeyinka Martins Adeyanju
Cybersecurity Analyst |
