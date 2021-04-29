# Introductory Researching Writeup - Easy 

This is a walkthrough of the "Introductory Researching" Room on <a href="https://tryhackme.com">TryHackMe.com</a>. 

**URL:** https://tryhackme.com/room/introtoresearch


<h1 style="color:Red">I encourage everyone to try completing the tasks without any help. Only use this sheet if you're stuck.</h1>

# Table of content
- [Task 1 - Introduction](#task-1---introduction)
- [Task 2 - Example Research Question](#task-2---example-research-question)
- [Task 3 - Vulnerability Searching](#task-3---vulnerability-searching)
- [Task 4 -  Manual Pages](#task-4---manual-pages)
- [Task 5 - Final Thoughts](#task-5---final-thoughts)



# Task 1 - Introduction:
Read the introduction:

```
No answer neeeded
```

# Task 2 - Example Research Question
**Tool used for this task: Google.com** 


In the Burp Suite Program that ships with Kali Linux, what mode would you use to manually send a request (often repeating a captured request numerous times)?
```
Repeater
```
What hash format are modern Windows login passwords stored in?
```
NTLM
```
What are automated tasks called in Linux?
```
Cron Jobs
```
What number base could you use as a shorthand for base 2 (binary)?
```
Base 16
```
If a password hash starts with $6$, what format is it (Unix variant)?
```
sha512crypt
```

# Task 3 - Vulnerability Searching
**Tool used for this task: exploit-db.com**

What is the CVE for the 2020 Cross-Site Scripting (XSS) vulnerability found in WPForms?
```
CVE-2020-10385
```
There was a Local Privilege Escalation vulnerability found in the Debian version of Apache Tomcat, back in 2016. What's the CVE for this vulnerability?
```
CVE-2016-1240
```
What is the very first CVE found in the VLC media player?
```
CVE-2007-0017
```
If you wanted to exploit a 2020 buffer overflow in the sudo program, which CVE would you use?
```
CVE-2019-18634
```

# Task 4 -  Manual Pages
**Tool used for this task: Linux man pages. Can be found by using the ```man``` command in your terminal**

SCP is a tool used to copy files from one computer to another.
What switch would you use to copy an entire directory?
```
-r
```
fdisk is a command used to view and alter the partitioning scheme used on your hard drive.
What switch would you use to list the current partitions?
```
-l
```
nano is an easy-to-use text editor for Linux. There are arguably better editors (Vim, being the obvious choice); however, nano is a great one to start with.
What switch would you use to make a backup when opening a file with nano?
```
-B
```
Netcat is a basic tool used to manually send and receive network requests. 
What command would you use to start netcat in listen mode, using port 12345?
```
nc -l -p 12345
```

# Task 5 - Final Thoughts
```
No answer needed.
```
