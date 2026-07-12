# Cowrie SSH Honeypot Deployment & Log Analysis

##  Project Objective
Deployed a Cowrie SSH honeypot in an isolated environment to simulate a vulnerable Secure Shell (SSH) server. This setup was designed to safely lure, log, and analyze unauthorized login attempts, brute-force attacks, and post-auth commands for security monitoring.

---

##  Tools & Environment
* **Honeypot OS:** Debian
* **Attacking OS:** Kali Linux
* **Honeypot Software:** Cowrie (SSH/Telnet honeypot)
* **Log Collection (Attempted):** Filebeat, Elasticsearch, Kibana (ELK Stack)

---

## Lab Deployment & Execution

### 1. Hardening & Security Best Practices
To ensure the honeypot didn't become a launchpad for actual system compromises, the following precautions were taken:

a.
* **Non-Root Execution:** 
Configured and ran the Cowrie service strictly under a low-privilege system user account to prevent privilege escalation.

b.
* **Port Configuration:** 
Verified that Cowrie was listening for connections on its default deployment port `2222` before routing traffic.

### 2. Starting the Honeypot Service
Initialized the virtual environment and started the Cowrie framework on the Debian machine:
```bash
source cowrie-env/bin/activate
cowrie start


3. Simulating Attacker Activity
a
​Connection Phase: 
Established a connection to the honeypot from the Kali Linux attacking machine using SSH protocols.

b.
​Interaction Phase: 
Generated simulated brute-force login attempts and executed common reconnaissance commands within the interactive terminal shell.


4. Observations & Results
a
​High Simulation:
The honeypot successfully mimicked a realistic Linux terminal environment, keeping the "attacker"(me) engaged.
b.
​Data Capture:
Cowrie successfully logged unauthorized credentials, captured session logs, and recorded every input command executed during the session.


