# DVWA Vulnerability Testing Lab

##  Project Objective
Deployed a controlled home lab environment to test, exploit, and analyze common web application vulnerabilities using Damn Vulnerable Web Application (DVWA). 

---

##  Tools and Environment
* **Host OS:** Debian
* **Attacking OS:** Kali Linux
* **Containerization:** Docker
* **Network Scanner:** Nmap
* **Exploitation Tools:** Firefox, Burp Suite

---

##  Lab Deployment and Execution

### 1. Setting Up the Target
The DVWA web server was deployed on the Debian host machine using Docker:

```bash
docker run --rm -it -p 8080:80 vulnerables/web-dvwa


2. Reconnaissance
​From the Kali Linux attacking machine, an active service enumeration scan was conducted to locate the target application:

nmap -sV 192.168.140.204 -p 8080

​Result: Discovered an open HTTP service running on port 8080.


​3.Vulnerability Exploitation
a.
​SQL Injection (SQLi): 
Successfully breached input validation limitations via the web UI, forcing the application to return unauthorized database records.

b.
​Cross-Site Scripting (XSS):
 Injected input payloads that executed directly within the client-side browser environment, demonstrating insufficient output encoding protections.



4.​Defense & Hardening
a.
​Network Isolation:
 Configured host-based firewall rules on the web server to restrict inbound traffic, permitting access strictly through service port 8080.


​5.Troubleshooting & Lessons Learned
a.

​The Challenge:
 Encountered initial connectivity issues where the attacking machine could not reach the DVWA container

b.
​The Fix:
 Identified a network bridging issue, reconfigured the virtual network adapters to ensure proper host-to-guest communication, and rebooted the host to successfully establish connection.


