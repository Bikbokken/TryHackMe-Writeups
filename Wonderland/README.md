


nmap -sC -sV $IP -oN nmapscan

└─$ nmap -sC -sV $IP -oN nmapscan
Starting Nmap 7.91 ( https://nmap.org ) at 2021-04-24 22:55 CEST
Nmap scan report for 10.10.162.25
Host is up (0.039s latency).
Not shown: 998 closed ports
PORT   STATE SERVICE VERSION
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 8e:ee:fb:96:ce:ad:70:dd:05:a9:3b:0d:b0:71:b8:63 (RSA)
|   256 7a:92:79:44:16:4f:20:43:50:a9:a8:47:e2:c2:be:84 (ECDSA)
|_  256 00:0b:80:44:e6:3d:4b:69:47:92:2c:55:14:7e:2a:c9 (ED25519)
80/tcp open  http    Golang net/http server (Go-IPFS json-rpc or InfluxDB API)
|_http-title: Follow the white rabbit.
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 15.29 seconds
   
wget "http://10.10.162.25/img/white_rabbit_1.jpg"
steghide extract -sf white_rabbit_1.jpg

gobuster dir -u http://$IP/ -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -o gobuster-scan
──(kali㉿kali)-[~/TryHackMe-Writeups/Wonderland]
└─$ gobuster dir -u http://$IP/ -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -o gobuster-scan
===============================================================
Gobuster v3.1.0
by OJ Reeves (@TheColonial) & Christian Mehlmauer (@firefart)
===============================================================
[+] Url:                     http://10.10.162.25/
[+] Method:                  GET
[+] Threads:                 10
[+] Wordlist:                /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
[+] Negative Status codes:   404
[+] User Agent:              gobuster/3.1.0
[+] Timeout:                 10s
===============================================================
2021/04/24 23:04:58 Starting gobuster in directory enumeration mode
===============================================================
/img                  (Status: 301) [Size: 0] [--> img/]
/r                    (Status: 301) [Size: 0] [--> r/]  
/poem                 (Status: 301) [Size: 0] [--> poem/]
/http%3A%2F%2Fwww     (Status: 301) [Size: 0] [--> /http:/www]
/http%3A%2F%2Fyoutube (Status: 301) [Size: 0] [--> /http:/youtube]
/http%3A%2F%2Fblogs   (Status: 301) [Size: 0] [--> /http:/blogs]  
/http%3A%2F%2Fblog    (Status: 301) [Size: 0] [--> /http:/blog]   
/**http%3A%2F%2Fwww   (Status: 301) [Size: 0] [--> /%2A%2Ahttp:/www]
/http%3A%2F%2Fcommunity (Status: 301) [Size: 0] [--> /http:/community]
/http%3A%2F%2Fradar   (Status: 301) [Size: 0] [--> /http:/radar]      
/http%3A%2F%2Fjeremiahgrossman (Status: 301) [Size: 0] [--> /http:/jeremiahgrossman]
/http%3A%2F%2Fweblog  (Status: 301) [Size: 0] [--> /http:/weblog]                   
/http%3A%2F%2Fswik    (Status: 301) [Size: 0] [--> /http:/swik]                     
                                                                                    
===============================================================
2021/04/24 23:21:00 Finished
===============================================================
                                                                 





python -m SimpleHTTPServer 2000


Files with capabilities:
/usr/bin/perl5.26.1 = cap_setuid+ep
/usr/bin/mtr-packet = cap_net_raw+ep
/usr/bin/perl = cap_setuid+ep




thm{******************************* at!} - root



thm{"*************** !"} -user
