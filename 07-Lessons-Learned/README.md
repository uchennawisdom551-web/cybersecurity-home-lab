# Lessons Learned

## Overview

Building this cybersecurity home lab provided practical experience in offensive security, defensive monitoring, Linux administration, troubleshooting, and technical documentation. Beyond learning individual tools, this project reinforced the importance of patience, problem-solving, and continuous learning in cybersecurity.

---

## Technical Skills Gained

Throughout this project, I strengthened my understanding of:

- Linux Administration
- Docker
- VirtualBox Networking
- DVWA
- Cowrie Honeypot
- Filebeat
- Elasticsearch
- Kibana
- Log Analysis
- Cybersecurity Documentation

---

## Challenges Encountered

### ELK Stack Configuration

Configuring Filebeat, Elasticsearch, and Kibana required multiple rounds of troubleshooting before logs appeared correctly.

**Resolution**

- Verified Filebeat configuration.
- Restarted required services.
- Checked Elasticsearch indices.
- Confirmed Kibana connectivity.

---

### Docker Resource Usage

Running multiple containers consumed significant storage and system resources.

**Resolution**

- Removed unused Docker images and containers.
- Managed available storage more efficiently.

---

### Virtual Machine Networking

Establishing communication between virtual machines required proper network configuration.

**Resolution**

- Verified VirtualBox network adapters.
- Tested connectivity between systems before proceeding.

---

### Linux Permissions

Several services required additional user permissions before functioning correctly.

**Resolution**

- Modified user groups.
- Corrected Linux file permissions where necessary.

---

## Key Takeaways

This project taught me that:

- Cybersecurity involves both attacking and defending systems.
- Proper documentation is as important as technical implementation.
- Troubleshooting is an essential cybersecurity skill.
- Linux knowledge forms the foundation of many cybersecurity tools.
- Security monitoring provides valuable visibility into attacker behavior.

---

## Future Improvements

Future enhancements to this home lab include:

- Suricata IDS
- Zeek Network Monitor
- Autopsy Digital Forensics
- SIEM Alerting Rules
- Additional vulnerable applications
- Expanded attack scenarios

---

## Final Reflection

This project significantly improved my confidence working with Linux, cybersecurity tools, and security monitoring solutions. It also strengthened my problem-solving skills by exposing me to real configuration challenges that required systematic troubleshooting and persistence. Building this lab has provided a strong foundation for future learning in cybersecurity and digital forensics.
