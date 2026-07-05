Objective 
-Deployed a Cowrie SSH honeypot to simulate a vulnerable SSH server and capture attacker login attempts and commands for security 
 monitoring.

Enviroment
-Kali Linux
-Cowrie Honeypot
-Debian
-SHH

Steps Taken
-Installed Cowrie
-Started the Cowrie Service using the command line: "Source cowrie-env/bin/activate"
-Verified it was listening for connections on port 2222 
-Ensured it wasnt being operated from the root account to prevent giving attackers escalated privilleges 
-Connected from the Kali attack machine
-Generated fake attacker activity 
-Captured login attempts and commands

Observations 
-log attempts were successfully captured by cowrie
including fake attack commands, generated session logs. Honey pot behaved like a real word secure shell server 

Major Challenges 
-Filebeat was configured to retrieve cowrie logs
-An attempt was made to foward cowrie logs into elasticresearch.service
-The logs did not appear on Kibana Dashboard despite troubleshooting
-As an aternative measure the raw cowrie log files were directly observed  on cowrie server
-This method also ensured I properly observed attacker activity and verify honeypots functional activity 
