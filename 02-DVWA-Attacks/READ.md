DVWA Attacks

Objective
Test common web application vulnerabilities using DVWA in a controlled home lab.

Vulnerabilities Tested
-SQL injection
-Cross-Site Scripting (XSS)

Tools Used 
-Kali Linux 
-DVWA
-Firefox/Browser

Lab Demonstrations 
-Spinned up dvwa web server on my host machine(debian) using the command line "docker run --rm -it -p 8080:80 vulnerables/web-dvwa"
- To perform web reconnaissance using the attacking machine ( kali ) 
- Ran " nmap -sV 192.168.140.204 -p 8080 " discovered open HTTP port, opened the website and performed xss/sql injections.
Results
-SQL injection successfully breached normal input validation, the application returned database records that shoudnt have been accessible
-The vulnerability highlighted the importance of paratemeterized queries and input validation

-For Cross-site-scripting, the application accepted and executed injected java script code 
-The injected script was displayed and executed in the browser
-This demonstrates how attackers can exploit insufficient input validation 
-The exercise ensures the importance of proper output coding and input validation


Defense Mechanism 
-A firewall file was configured on the web server to permit access to only the service port 8080 (HTTP)

Challenges 
-Had trouble spinning up the dvwa website at first because i wasn't puting in the correct ip address

Corrections
-Rebooted the host machine after reconfigurating its network adapter to get a suitable one that can be used for the exercise and it worked out successfully.


