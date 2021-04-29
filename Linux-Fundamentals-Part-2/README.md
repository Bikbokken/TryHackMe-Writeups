# Linux Fundamentals Part 2 Writeup - Easy 

This is a walkthrough of the "Linux Fundamentals Part 2" room on <a href="https://tryhackme.com">TryHackMe.com</a>. 

**URL:** https://tryhackme.com/room/linux2


<h1 style="color:Red">I encourage everyone to try completing the tasks without any help. Only use this sheet if you're stuck.</h1>

# Table of content
- [Task 1 - Intro](#task-1---intro)
- [Task 2 - SSH - Intro](#task-2---ssh---intro)
- [Task 3 - Putty and SSH](#task-3---putty-and-ssh)
- [Task 4 - [Section 4: Linux Operators]: "&&"](#task4)
- [Task 5 - [Section 4: Linux Operators]: "&"](#task5)
- [Task 6 - [Section 4: Linux Operators]: "$"](#task6)
- [Task 7 - [Section 4: Linux Operators]: "|"](#task7)
- [Task 8 - [Section 4: Linux Operators] - ";"](#task8)
- [Task 9 - [Section 4: Linux Operators]: ">"](#task9)
- [Task 10 - [Section 4: Linux Operators]: ">>"](#task10)
- [Task 11 - Binary - shiba2](#task-11---binary---shiba2)
- [Task 12 - [Section 5 - Advanced File Operations]: Intro](#task-12---section-5---advanced-file-operations-intro)
- [Task 13 - [Section 5 - Advanced File Operators]: A bit of background.](#task-13---section-5---advanced-file-operators-a-bit-of-background)
- [Task 14 - [Section 5: Advanced File Operations]: chown](#task-14---section-5-advanced-file-operations-chown)
- [Task 15 - [Section 5: Advanced File Operations]: chmod](#task-15---section-5-advanced-file-operations-chmod)
- [Task 16 - [Section 5: Advanced File Operations]: rm](#task-16---section-5-advanced-file-operations-rm)
- [Task 17 - [Section 5: Advanced File Operations]: mv](#task-17---section-5-advanced-file-operations-mv)
- [Task 18 - Linux Fundamentals 3](#task-18---linux-fundamentals-3)





# Task 1 - Intro: 
Read the above.
```
No answer neeeded
```

Deploy the machine attached to this task!
```
No answer neeeded - Deploy the machine
```


# Task 2 - SSH - Intro
Read the above.
```
No answer neeeded
```

# Task 3 - Putty and SSH 
SSH into the server
```
No answer neeeded - SSH into the server 
```
<div id="task4"></div>

# Task 4 - [Section 4: Linux Operators]: "&&"
Read the above.
```
No answer neeeded
```
<div id="task5"></div>

# Task 5 - [Section 4: Linux Operators]: "&"
Read the above.
```
No answer neeeded
```

<div id="task6"></div>

# Task 6 - [Section 4: Linux Operators]: "$"
How would you set nootnoot equal to 1111
```
export nootnoot=1111
```
What is the value of the home environment variable
```
/home/shiba2
```
<div id="task7"></div>

# Task 7 - [Section 4: Linux Operators]: "|"
Read the above.
```
No answer neeeded
```
<div id="task8"></div>

# Task 8 - [Section 4: Linux Operators] - ";"
Read the above.
```
No answer neeeded
```
<div id="task9"></div>

# Task 9 - [Section 4: Linux Operators]: ">"
How would you output twenty to a file called test
```
echo twenty > test
```
<div id="task10"></div>

# Task 10 - [Section 4: Linux Operators]: ">>"
Read the above.
```
No answer neeeded
```

# Task 11 - Binary - shiba2
What is shiba3's password?
```
└─$export test1234=$USER
└─$echo $test1234
└─$./shiba2
h**p*noot*****

```

# Task 12 - [Section 5 - Advanced File Operations]: Intro
Read the above.
```
No answer neeeded
```

# Task 13 - [Section 5 - Advanced File Operators]: A bit of background.
Read the above.
```
No answer neeeded
```

# Task 14 - [Section 5: Advanced File Operations]: chown
How would you change the owner of file to paradox
```
chown paradox file
```

What about the owner and the group of file to paradox
```
chown paradox:paradox file
```

What flag allows you to operate on every file in the directory at once?
```
-R
```

# Task 15 - [Section 5: Advanced File Operations]: chmod

What permissions mean the user can read the file, the group can read and write to the file, and no one else can read, write or execute the file?
```
460
```
What permissions mean the user can read, write, and execute the file, the group can read, write, and execute the file, and everyone else can read, write, and execute the file.
```
777
```


# Task 16 - [Section 5: Advanced File Operations]: rm
What flag deletes every file in a directory
```
-r
```
How do you suppress all warning prompts
```
-f
```

# Task 17 - [Section 5: Advanced File Operations]: mv
How would you move file to /tmp
```
mv file /tmp
```

# Task 18 - Linux Fundamentals 3
Join the Linux Fundamentals 3 room, and finish learning Linux: https://tryhackme.com/room/linux3
```
No answer needed
```




Continue to Linux Fundamentals 3 writeup <a href="../Linux-Fundamentals-Part-3/README.md">here</a>

