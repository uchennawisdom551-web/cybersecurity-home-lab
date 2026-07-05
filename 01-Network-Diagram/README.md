Network Diagram

Objective

Design a home lab capable of simulating attacks, collecting logs, and monitoring security events.

Components

- Kali Linux (Attacker)
- DVWA (Vulnerable Web Application)
- Cowrie SSH Honeypot
- Filebeat
- Elasticsearch
- Kibana

 Network Flow

Kali Linux
        │
        ▼
DVWA / Cowrie
        │
        ▼
Filebeat
        │
        ▼
Elasticsearch
        │
        ▼
Kibana Dashboard

Evidence

The network diagram used in this project is included in this folder.
