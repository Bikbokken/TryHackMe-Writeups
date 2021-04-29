# The find command - Easy 

This is the "The find command" Room on <a href="https://tryhackme.com">TryHackMe.com</a>. 

**URL:** https://tryhackme.com/room/thefindcommand


<h1 style="color:Red">I encourage everyone to try completing the tasks without any help. Only use this sheet if you're stuck.</h1>

# Table of Contents
- [Task 1 - Start finding](#task-1---start-finding)
- [Task 2 - Be more specific](#task-2---be-more-specific)
- [Task 3 - Know exactly what you're looking for](#task-3---know-exactly-what-youre-looking-for)
- [Task 4 - Have you found it?](#task-4---have-you-found-it)


# Task 1 - Start finding
Read and follow the instructions.
```
No answer neeeded
```

# Task 2 - Be more specific
Find all files whose name ends with ".xml"
```
find / -type f -name "*.xml"
```
Find all files in the /home directory (recursive) whose name is "user.txt" (case insensitive)

```
find /home -type f -iname user.txt
```

Find all directories whose name contains the word "exploits"
```
find / -type d -name "*exploits*"
```


# Task 3 - Know exactly what you're looking for
Find all files owned by the user "kittycat"
```
find / type -f -user kittycat
```

Find all files that are exactly 150 bytes in size
```
find / -type f -size 150
```
Find all files in the /home directory (recursive) with size less than 2 KiB’s and extension ".txt"
```
find /home -type f -size 2 -name "*.txt"
```
Find all files that are exactly readable and writeable by the owner, and readable by everyone else (use octal format)
```
find / -type f -perm 644
```
Find all files that are only readable by anyone (use octal format)
```
find / -type f -perm /444
```
Find all files with write permission for the group "others", regardless of any other permissions, with extension ".sh" (use symbolic format)
```
find / -type f -perm -o=w -name “*.sh
```
Find all files in the /usr/bin directory (recursive) that are owned by root and have at least the SUID permission (use symbolic format)
```
find /usr/bin -type f -user root -perm -u=s
```
Find all files that were not accessed in the last 10 days with extension ".png"
```
find / -type f -time +10 -name "*.png"
```
Find all files in the /usr/bin directory (recursive) that have been modified within the last 2 hours
```
find /usr/bin -type f -mmin -120
```

# Task 4 - Have you found it?
You are now better equipped to find anything you’re looking for in a filesystem.
```
No answer needed
```


