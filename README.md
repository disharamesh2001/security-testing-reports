# Security Testing Reports

This repository contains a manual penetration test report for an example/demo web application (Acunetix).  
The report documents identified vulnerabilities, reproduction steps, screenshots, and recommended remediations.

---

## 📂 Contents

| File / Folder | Description |
|---------------|-------------|
| `Acunetix_Penetration_Test_Report.pdf` | PDF version of the penetration test report. Contains findings, sanitized screenshots, PoCs (where safe), and remediation recommendations. |

---

## 🔎 Executive Summary
This report is a manual security assessment performed against a demo Acunetix web application environment for educational and training purposes. The assessment focuses on OWASP-relevant issues and documents both the verification steps and suggested fixes.

## ⚠️ Key Findings
The most important issues identified in the assessment include:
- **Weak Account Lockout / Brute Force Protection** — insufficient lockout or throttling for repeated authentication attempts.  
- **Cryptographic Failures** — insecure use or configuration of cryptographic functions (e.g., weak TLS settings, insecure storage).  
- **SQL Injection** — injectable parameters allowing unauthorized database interactions (sanitized PoC included).  
- **Broken Access Control** — improper restrictions allowing unauthorized actions.  
- **Insecure Direct Object Reference (IDOR)** — direct access to objects (files, records) without proper authorization checks.

Each finding in the report contains:
- A concise description of the vulnerability  
- Step-by-step reproduction (sanitized)  
- Evidence (screenshots / request-response snippets with sensitive data redacted)  
- Severity and business impact  
- Practical remediation recommendations

---

## 🧰 Tools & Techniques Used
- Manual testing techniques (crafted HTTP requests, browser DevTools)  
- Vulnerability validation and evidence collection (screenshots, request/response snippets)  
- Note: Acunetix was used as the demo target; testing performed in an authorized demo/training environment.

---

## 📘 Notes & Safety
- This work was performed in an **authorized demo/training environment**. No real client systems were tested.  
- All screenshots and request/response examples have been **sanitized or redacted** to remove sensitive information.  
- The report is shared **for educational purposes only**.

---

## How to View
- Open `Acunetix_Penetration_Test_Report.pdf` to read the full report and view screenshots. GitHub supports in-browser PDF preview.

---

*Author: Disha Ramesh*  

---
