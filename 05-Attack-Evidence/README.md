# Attack Evidence

## 1. Nmap Reconnaissance
**Screenshot:** nmap_reconnaissance.png

**Objective:** Identify open ports and running services on the target machine.

**Observation:** The scan revealed the active services running on the target, confirming that the web server was reachable before proceeding with further testing.

---

## 2. SQL Injection
**Screenshot:** sql_injection.png

**Objective:** Test the DVWA application for SQL Injection vulnerabilities.

**Observation:** The SQL payload was accepted by the application and successfully bypassed the intended input validation, confirming that the application was vulnerable to SQL Injection.

---

## 3. Reflected Cross-Site Scripting (XSS)
**Screenshot:** reflected_xss.png

**Objective:** Test the application for reflected XSS by entering test input into the vulnerable field.

**Observation:** The input was reflected back by the application without proper validation, indicating that the application was vulnerable to Reflected XSS.

---

## 4. Stored Cross-Site Scripting (XSS)
**Screenshot:** stored_xss.png

**Objective:** Test the application for stored XSS by submitting input through the vulnerable form.

**Observation:** The submitted input was saved by the application and displayed whenever the affected page was accessed, confirming that the application was vulnerable to Stored XSS.
