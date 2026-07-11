#### Nmap Scan

We received 2 open ports by scannning using Nmap:

1. **Port 22 (ssh)**

2. **port 80 (http)**



We open the site using http and recieve a page. There is nothing much on the page. 

We do get a username from the **source code of the page**, it is commented, we can click this particular command on our keyboard to open source code of the page:

```Keyboard
Ctrl + U
```

---

#### Gobuster tool

we use this following command using gobuster tool to get directories available on the web server:

```Terminal
gobuster dir -u http://$IP_ADDR -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -x '.js,.html,css,.txt,.cgi,.php'
```


we go to a page where we get a **portal login page** from the directory enumeration.

we use the username we got from the source page and **password is stored in a .txt file** (found using gobuster)

**We get the dashboard!!!**

---

#### Reconnaissance

There is a panel on the page where we can **execute linux commands**.

We can get a lot of information by listing the files and directories using **ls** command.

There is a **secret txt file**, we can open by using the txt file as a parameter of the address.

**We get our first flag!!**


we can execute commands to check if python is working on the panel or not.

python is not but **python3** is working.

---

#### Reverse shell

We can get a reverse shell using python. Here are the steps as follows:

1. Go to pentest monkey reverse shell cheat sheet

2. Go to python, and change the ip address to the attacker's ip address and the desired port.

3. open a netcat listener by the following command:

```Terminal
nc -nvlp $PORT
```

4. Execute the python command on the command panel on the web page.

5. You will get the shell on the Terminal !!

---

#### Enumeration

After Getting the shell, we can check for the flags.

Best is to check user's files and directories **first!**

We list files on the user 'rick' using the following command on the shell:

```Terminal
ls /home/rick
```

**There is a file containing second flag!!**

---

#### Privileges

We can check our sudo privileges using this command:

```Terminal
Sudo -l
```

The output shows us that we basically have all the root privileges if we use sudo:

```
(ALL) NOPASSWD: ALL
```


we can check the root user's files and directories.

**There is a last and final flag there!!**