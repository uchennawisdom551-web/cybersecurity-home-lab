Objective

-Set up the ELK Stack to collect, store, and visualize security logs from the home lab.

Components

-Elasticsearch
-Kibana
-Filebeat


Steps Taken

-Installed Elasticsearch
-Installed Kibana
-Installed and configured Filebeat
-Configured Filebeat to monitor Cowrie log files
-Started all services required 
-Attempted to forward logs into Elasticsearch
-Accessed Kibana to verify indexed data

Challenges Encountered
 This is where something troublesome really happened 
-Filebeat was successfully configured to parse log files
-Despite troubleshooting, Cowrie logs were not successfully indexed into Elasticsearch
-As a result, the expected data did not appear in the Kibana dashboard
-To continue the project, raw Cowrie log files on the server were used to observe attacker activity


Lessons Learned
-Proper configuration of Filebeat and Elasticsearch is essential for log ingestion
-Troubleshooting log pipelines is an important cybersecurity skill
'Even when dashboards fail, raw log analysis remains valuable
