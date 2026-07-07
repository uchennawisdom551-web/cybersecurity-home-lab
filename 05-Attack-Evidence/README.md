# Attack Evidence

## 1. Nmap Reconnaissance
 Screenshot: nmap_reconnaissance.png

- Objective: Identify open ports and services on the target.
- Observation: The scan identified the web server running on the target machine


## 2. SQL Injection
Screenshot: sql_injection.png

- Objective: Test the DVWA application for SQL Injection.
- Observation: The application accepted the malicious input, confirming that it was vulnerable to SQL Injection.

---

## 3. Stored Cross-Site Scripting (XSS)
Screenshot: stored_xss.png

- Objective: Test the DVWA application for Stored XSS.
- Observation: The injected JavaScript payload was saved by the application and executed whenever the affected page was loaded, confirming the Stored XSS vulnerability.
