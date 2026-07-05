# ELK Stack

## Objective

The goal of this stage was to collect and visualize logs generated during my home lab attacks using Elasticsearch, Kibana, and Filebeat.

## What I Did

- Installed Elasticsearch and Kibana.
- Installed and configured Filebeat.
- Configured Filebeat to monitor Cowrie log files.
- Started all the required services.
- Tried forwarding the Cowrie logs to Elasticsearch.
- Checked Kibana to see if the logs were indexed.

## What Happened

This was probably the most challenging part of the project.

Filebeat was able to detect and read the Cowrie log files, but I couldn't get the logs to appear in Elasticsearch or Kibana despite trying different configurations and troubleshooting for quite a while.

Instead of abandoning the project, I decided to analyze the raw Cowrie log files directly from the server. Although the dashboard wasn't working as expected, I was still able to monitor attacker activity and understand what was happening.

## What I Learned

This experience taught me that building security monitoring systems is not always straightforward. Small configuration mistakes can stop an entire logging pipeline from working.

More importantly, I learned that troubleshooting is part of cybersecurity. Even when automation fails, understanding how to work with raw logs is an important skill.
