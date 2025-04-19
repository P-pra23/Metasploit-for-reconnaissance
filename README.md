# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:
Find out the ip address of the attackers system

## OUTPUT:

![image](https://github.com/user-attachments/assets/f39e8ea0-b4b0-4578-9a95-c63b7c2dc390)

Before beginning, set up the Metasploit database by starting the PostgreSQL server and initialize msfconsole database as follows: systemctl start postgresql msfdb init Invoke msfconsole:
![image](https://github.com/user-attachments/assets/9de0b1b9-0850-4d1d-b6fd-9ff56cc6e427)


Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.
![image](https://github.com/user-attachments/assets/65453478-08ed-40db-979a-f76d3d02843b) 
Port Scanning: Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000). msf > nmap -sT 192.168.1810/24 -p1-1000 OUTPUT:

 ![image](https://github.com/user-attachments/assets/16dae656-4edc-41fc-ad10-e9173fdf27b1)

multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules. cd /usr/share /metasploit-framework/modules/auxiliary kali > ls -l output:
![image](https://github.com/user-attachments/assets/5715f7e4-6c19-4d6e-aa88-6cce3748b258)
Search is a powerful command in Metasploit that you can use to find what you want to locate. msf >search name:Microsoft type:exploit output:
![image](https://github.com/user-attachments/assets/de8f953d-d64b-4917-b587-b0af76014185)
The info command provides information regarding a module or platform,

![image](https://github.com/user-attachments/assets/9b90a5db-9833-47e8-a00b-92c57464dbf1)

MYSQL ENUMERATION Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port. db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
![image](https://github.com/user-attachments/assets/4d31d846-b329-49c9-9f23-134afc91fcef)

Use the search option to look for an auxiliary module to scan and enumerate the MySQL database. search type:auxiliary mysql use the auxiliary/scanner/mysql/mysql_version module by typing the module name or associated number to scan MySQL version details. use 11 Or: use auxiliary/scanner/mysql/mysql_version
![image](https://github.com/user-attachments/assets/9ad96ebc-d78e-49f7-a2b8-0ce3281e4daf)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
