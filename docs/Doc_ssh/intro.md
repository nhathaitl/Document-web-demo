# Getting started - SSH

This is the demo made by Nhat Thai .TL

## The Defination of SSH

> Secure Shell (SSH) is a cryptographic network protocol used to secure
remote connections between computers. It is commonly used to log in to
remote servers, execute commands, and transfer files between computers.

## Step to ssh to host

At server side: install ssh open server if you still yet. If your OS is
the Debian then you can you this command

```bash
sudo apt-get install openssh-server
```
At client: type this cmd into terminal:
```bash
ssh <user>@<IP_host>
```
user: is the username of server. If superuser then root IP_host : it\'s
mean the IP_v4 of the server After step 2 then you\'ll type the password
of the host Now let\'s enjoy your result !!

## Save Password via VS-Code

For those trying to connect through Vscode Remote SSH Extension steps
provided at
<https://code.visualstudio.com/docs/remote/troubleshooting#_ssh-tips>

**For Windows(Host) \--\> Linux(Remote)**

-   Create an SSH .pub key in your windows `ssh-keygen -t rsa -b 4096`
-   Copy the contents of the .pub key (**default path
    C:Usersusername/.ssh/id_rsa.pub**)
-   SSH into Remote machine and append the contents of the pub key in
    authorized keys `echo "pub-key" >> ~/.ssh/authorized_keys`

## Troubleshoot

If you cannot asscess root user althought enter correct password then:

* open file config of openssh:
```bash
sudo vi /etc/ssh/sshd_config
```

* Need to change the #PermitRootLogin prohibit-password setting to yes:
```bash
sudo sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config
```

* then, restart ssh service:
```bash
sudo service ssh restart
```

* Change root\'s user password:
```bash
sudo passwd
[sudo] password for linuxconfig: 
Enter new UNIX password: 
Retype new UNIX password: 
passwd: password updated successfully 
```

* To make sure u can disable firewall:
```bash
sudo ufw allow ssh
```