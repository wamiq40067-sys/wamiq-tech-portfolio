#### Nmap Scan ####

We need to Scan the machine to know the open ports, in this case we use stealthy scan:

```Terminal
nmap -sS -sV $IP_addr
```

After our scan , we get 3 open ports:
**port 21 (ftp)**

**port 22 (ssh)**

**port 80 (http)**


#### ftp ####

We ftp into the machine using ftp command.

```Terminal
ftp $TARGET_IP_ADDR $PORT
```

Guessed the username as **anonymous** and got access.

Downloaded the file **task.txt** and **locks.txt** using **get** command.



#### Hydra ####


Now that we know the username and got a list of passwords in locks.txt, we can Brute force into it using Hydra By SSH.


Command goes as follows:

```Terminal
hydra -l (username) -P /home/kali/Desktop/locks.txt ssh://$IP_ADDR -t 4
```


By Brute forcing, we receive the password required to login through ssh.

After we login, we immediately get the flag in user.txt.



#### Privilege Escalation ####

To know what sudo privileges the user has, we type this command:

```Terminal
sudo -l
```

This is the permission user has :

```Terminal
User (user) may run the following commands on ip-($IP):
    (root) /bin/tar
```



We can visit gtfobins to abuse this privilege.



Here are the steps to use the command necessary to abuse them:

1. Go to gtfobins.

2. filter **tar**.

3. Go to sudo in shell section.

4. copy and paste it in the terminal using **sudo**.


We get the root shell.

The flag is in root.txt, we can use find command to find it

```Terminal
find / -name root.txt
```