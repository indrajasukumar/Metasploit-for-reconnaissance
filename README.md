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

## Program:
Find out the ip address of the attackers system


![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/c518a95a-8d56-4e4d-9d91-b14dcc7d1daf)

## Invoke msfconsole:

## OUTPUT:
Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/0b84a946-6adc-4e4f-8a31-287266c32ae3)

## Port Scanning Output:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000). msf > nmap -sT 192.168.1810/24 -p1-1000


![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/8f3485a8-601b-434e-88c3-eed8abf133c9)







## OUTPUT:

![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/dfc332c7-adc7-4cce-a48a-3ba6adc0acad)


the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.

scan the targets with the command db_nmap as follows. msf > db_nmap 192.168.181.0/24

## output
![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/6a52c2ea-b6cb-45b8-82b0-1db834e138d6)

Metasploit has a multitude of scanning modules built in. If we open another terminal, we can navigate to Metasploit's auxiliary modules and list all the scanner modules. cd /usr/share /metasploit-framework/modules/auxiliary kali > ls -l

## output

![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/e5a228ed-5a5f-486a-b97f-c0c8f188b896)


Search is a powerful command in Metasploit that you can use to find what you want to locate. msf >search name:Microsoft type:exploit

The info command provides information regarding a module or platform

## output:
![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/d7d63847-6d18-4cf3-91b8-985a9a14755d)


Before beginning, set up the Metasploit database by starting the PostgreSQL server and initialize msfconsole database as follows: systemctl start postgresql msfdb init

## MYSQL ENUMERATION:
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port. db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

## output:


![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/3cd1ea33-da14-41e9-8010-ecf3418bc6b5)

## output:

![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/85322341-9bf2-4164-8bcf-c14efed5cde6)

set the PASS_FILE parameter to the wordlist path available inside /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt Then, specify the IP address of the target machine with the RHOSTS command. set RHOSTS Set BLANK_PASSWORDS to true in case there is no password set for the root account. set BLANK_PASSWORDS true


![image](https://github.com/indrajasukumar/Metasploit-for-reconnaissance/assets/145115195/35309c24-5030-4305-ac8c-df4a2c46a8f2)




## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
