# Linux Fundamentals Part 3 - Easy 

This is the "Linux Fundamentals Part 3" room on <a href="https://tryhackme.com">TryHackMe.com</a>. 

**URL:** https://tryhackme.com/room/linux3


<h1 style="color:Red">I encourage everyone to try completing the tasks without any help. Only use this sheet if you're stuck.</h1>


# Table of content
- [Task 1 - Intro](#task-1---intro)
- [Task 2 - [Section 5: Advanced File Operations] - cp](#task-2---section-5-advanced-file-operations---cp)
- [Task 3 - [Section 5: Advanced file Operations] - cd && mkdir](#task-3---section-5-advanced-file-operations---cd--mkdir)
- [Task 4 - [Section 5: Advanced File Operations] ln](#task-4---section-5-advanced-file-operations-ln)
- [Task 5 - [Section 5 - Advanced File Operations]: find](#task-5---section-5---advanced-file-operations-find)
- [Task 6 - [Section 5: Advanced File Operations] - grep](#task-6---section-5-advanced-file-operations---grep)
- [Task 7 -  Binary - Shiba3](#task-7----binary---shiba3)
- [Task 8 - [Section 6: Miscellaneous]: Intro](#task-8---section-6-miscellaneous-intro)
- [Task 9 - [Section 6: Miscellaneous]: sudo](#task-9---section-6-miscellaneous-sudo)
- [Task 10 - [Section 6: Miscellaneous]: Adding users and groups](#task-10---section-6-miscellaneous-adding-users-and-groups)
- [Task 11 - [Section 6: Miscellaneous]: nano](#task-11---section-6-miscellaneous-nano)
- [Task 12 - [Section 6: Miscellaneous]: Basic shell scripting](#task-12---section-6-miscellaneous-basic-shell-scripting)
- [Task 13 - [Section 6: Miscellaneous]: Important Files and Directories](#task-13---section-6-miscellaneous-important-files-and-directories)
- [Task 14 - [Section 6 - Miscellaneous]: Installing packages(apt)](#task-14---section-6---miscellaneous-installing-packagesapt)
- [Task 15 - [Section 6: Miscellaneous]: Processes](#task-15---section-6-miscellaneous-processes)





# Task 1 - Intro 
Read the above.
```
No answer neeeded
```

Deploy the machine attached to this task!
```
No answer neeeded - Deploy the machine
```


# Task 2 - [Section 5: Advanced File Operations] - cp
Read the above.
```
No answer neeeded
```

# Task 3 - [Section 5: Advanced file Operations] - cd && mkdir
Using relative paths, how would you cd to your home directory.
```
cd ~
```
Using absolute paths how would you make a directory called test in /tmp
```
mkdir /tmp/test
```

# Task 4 - [Section 5: Advanced File Operations] ln
How would I link /home/test/testfile to /tmp/test
```
ln /home/test/testfile /tmp/test
```




# Task 5 - [Section 5 - Advanced File Operations]: find
How do you find files that have specific permissions?
```
-perm
```
How would you find all the files in /home
```
find /home
```
How would you find all the files owned by paradox on the whole system
```
find / -user paradox
```


# Task 6 - [Section 5: Advanced File Operations] - grep
What flag lists line numbers for every string found?
```
-n
```
How would I search for the string boop in the file aaaa in the directory /tmp
```
grep boop /tmp/aaaa
```

# Task 7 -  Binary - Shiba3
What is shiba4's password
```
└─$ find /* | grep shiba4
└─$ /opt/secret/shiba4
**t**34
```

# Task 8 - [Section 6: Miscellaneous]: Intro
Read the above.
```
No answer neeeded
```

# Task 9 - [Section 6: Miscellaneous]: sudo
How do you specify which user you want to run a command as.
```
-u
```
How would I run whoami as user jen?
```
sudo -u jen whoami
```
How do you list your current sudo privileges(what commands you can run, who you can run them as etc.)    
```
-l
```

# Task 10 - [Section 6: Miscellaneous]: Adding users and groups
How would I add the user test to the group test

```
sudo usermod -a -G test test
```
# Task 11 - [Section 6: Miscellaneous]: nano
Read the above.
```
No answer neeeded
```
# Task 12 - [Section 6: Miscellaneous]: Basic shell scripting
Read the above.
```
No answer neeeded
```
# Task 13 - [Section 6: Miscellaneous]: Important Files and Directories
Read the above.
```
No answer neeeded
```
# Task 14 - [Section 6 - Miscellaneous]: Installing packages(apt)
Read the above.
```
No answer neeeded
```
# Task 15 - [Section 6: Miscellaneous]: Processes
Read the above.
```
No answer neeeded
```