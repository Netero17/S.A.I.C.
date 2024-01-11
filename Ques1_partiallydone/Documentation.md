## first changed network of vm to bridged Adapter in order to connect the vm to internet (why: Bridge mode allows your VM to act as its own device on your network, with its own IP address)

## found ip address of the web hosting server in guest mode > connection_information : lets say == ipaddr
![image](https://github.com/Netero17/S.A.I.C./assets/126668078/c8f731c2-2f3a-4f77-b1b7-3df9ebbcb474)

## scanning for all services hosted `sudo nmap -sC -sV -O -p- -oA` , result:
Nmap scan report for 192.168.29.160
Host is up (0.0025s latency).
Not shown: 65534 filtered tcp ports (no-response)
PORT   STATE SERVICE VERSION
80/tcp open  http    Apache httpd 2.2.22 ((Ubuntu))
|_http-title: Xenia (LinuxFox)
|_http-server-header: Apache/2.2.22 (Ubuntu)
| http-robots.txt: 5 disallowed entries 
|_/ange1 /angel1 /nothing /tmp /uploads
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: bridge|general purpose|switch
Running (JUST GUESSING): Oracle Virtualbox (96%), QEMU (91%), Bay Networks embedded (86%)
OS CPE: cpe:/o:oracle:virtualbox cpe:/a:qemu:qemu cpe:/h:baynetworks:baystack_450
Aggressive OS guesses: Oracle Virtualbox (96%), QEMU user mode network gateway (91%), Bay Networks BayStack 450 switch (software version 3.1.0.22) (86%)
No exact OS matches for host (test conditions non-ideal).

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 129.75 seconds

## found : 
-80/tcp open
-http-server-header: Apache/2.2.22 (Ubuntu)

## after visiting http://ipaddr i found a website

## using `python3 dirsearch.py -u http://192.168.29.160` searched for hidden directory
### search result :



### found :
- an encrypted zip file named Backup.zip on
  
  cracked the password of Backup.zip 
- lots of uri on robots.txt
  on the inspectpage of one of the uri's `/nothing` in robots.txt found :
`#my secret pass
xenia
tux
freedom
password
diana
helloworld!
iloveroot`
![image](https://github.com/Netero17/S.A.I.C./assets/126668078/c7759aea-610c-4bc5-8df0-45795f4accbf)

  
  
  
  
