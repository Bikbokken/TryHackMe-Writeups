# Hydra Writeup - Easy 

This is a walkthrough of the "Hydra" Room on <a href="https://tryhackme.com">TryHackMe.com</a>. 

**URL:** https://tryhackme.com/room/hydra


<h1 style="color:Red">I encourage everyone to try completing the tasks without any help. Only use this sheet if you're stuck.</h1>


# Task 1 - Hydra Introduction
Read the above and have Hydra at the ready.
```
No answer needed
```


# Task 2 - Using Hydra
**Use Hydra to bruteforce molly's web password. What is flag 1?**

The webpage on http://MACHINE_IP shows a login form, where you need to provide a username and password. We're going to use ``hydra`` as our bruteforcing tool, to bruteforce the password for the user ``molly``.

First we're going to find and analyse the POST request that is sent to the server, when trying to log in. We can find the POST request, by using the tab "Network" in dev tools that is built in your browser.
1. Open devtools by right clicking on the webpage and click "Inspect Element" *(can depend on the browser you're using, but it's probably the last option when right clicking on a webpage.)"*
2. Click on the "Network" tab within devtools.
3. Now type some random values into the username and password field and observe the POST request that is coming. 
4. Click on the POST request.
5. Click on "Request" in the right side of the page, after clicking on the POST request.
6. Copy the request payload and save it. (username=test&password=test)
7. Copy the login page link and save it. (http://MACHINE_IP/login)
8. Now copy the login failed message that is showing up and save it. (Your username or password is incorrect.)

Now you have all the information you need to perform a bruteforce attack.
```bash
└─$ hydra -l molly -P /usr/share/wordlists/rockyou.txt <MACHINE_IP> http-post-form "/login:username=^USER^&password=^PASS^:F=Your username or password is incorrect." -V
```
`-l` = provide the username, remember this is only a single username. If you want to use a user list, you need to use a big `-L` instead of `-l`

`-P` = provide the password list, remember this is a password list. If you want to use a single password, you need to use a small `-p` instead of `-P`.

`http-post-form` = indicates the type of form, in this case it's post. If

`/login:username=^UESR^&password=^PASS^` = As you noted before, the login page is on the `/login` page and as you also noted before, the request payload was `username=test&password=test`. But replacing the `test` username parameter with a `^USER^` which uses the `-l` or `-L` data and replacing the `test` password parameter with a `^PASS^` which again uses the `-p` or `-P` data.

`:F` = If this word appears on the page, the credentials are incorrect. `:F=Your username or password is incorrect.` which is the login failed message you saved before.

`-V` = Verbose output for every attempt. That means it prints every attempt it makes logging in.

After running the command from above, you will find the password is `sun****` for the user `molly`. Logging in with the credentials, you'll find the flag.



**Use Hydra to bruteforce molly's SSH password. What is flag 2?**
This process is more simple.


```bash
└─$ hydra -l molly -P /usr/share/wordlists/rockyou.txt ssh://MACHINE_IP
```
`-l` = provide the username, remember this is only a single username. If you want to use a user list, you need to use a big `-L` instead of `-l`

`-P` = provide the password list, remember this is a password list. If you want to use a single password, you need to use a small `-p` instead of `-P`.

Instead of using `http-post-form` and so on, you're able to only type the prefix ``ssh://`` to the IP. Hydra will automatically know that you're trying to bruteforce a SSH server. 

`-V` = Verbose output for every attempt. That means it prints every attempt it makes logging in.

After running the command from above, you will find the password is `but******` for the user `molly`. Logging in with the credentials on the SSH server, you'll find the flag, by using the command `cat flag2.txt`. 
