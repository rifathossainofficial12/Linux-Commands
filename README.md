# Linux-Commands
Linux basic and advance command for learning and practicing linux.

# Linux commands cheat sheet
a beginner- firendly Linux Commands cheat sheet for system administration, networking. and ethical hacking.

---

#Table of contents

| No | Topic |

| 1 | [Navigation and File Management](#Navigation-and-File-Management) |

| 2 | [User and Permission Management](#User-and-Permission-Management) |

| 3 | [Networking Commands](#Networking-commands) |

| 4 | [File Search and Manipulation](#File-Search-and-Manipulation) |

| 5 | [Privilege Escalation and Enumeration](#Privilege-Escalation-and-Enumeration) |

| 6 | [Tool Usage and Exploitation](#Tool-Usage-and-Exploitation) |

---

# Navigattion and File Management

| Command | Description |

|------------|-----------------|

|`pwd`| (print working directory) This command is used to show the current directory form terminal |

Ex: pwd

|`ls`| (list) this command is used to show directory contents. |

Ex: ls

|`ls -ls`| this command is used to show directory contents and details of contents like permission, file type, file create date time etc. |

Ex : ls -la

|`cd`| this command is used for changing directory |

Ex: cd /home/kali/desktop

|`cd folder_name`| This command is used to enter a specific directory. |

Ex : cd Music

|`cp`| this command is used for copying files of directories. |

Ex : cp file.txt /desktop/

|`mv`| this command is used for the move of rename files and directories. |

Ex : mv oldname.txt newname.txt

|`rm`| this command is used for removing files and directories. |

Ex : rm file.txt

|`rm -r`| Use this command to remove the directory and everything inside it. |

Ex : rm -f file.txt 

|`rm -rf`| Use this command to remove the directory and everything inside it forcefully. |

Ex : rm -rf file.txt

|`cat`| use this command to see file contents.  |

Ex: cat file.txt

|`nano / vim`| use this command for edit text files|

Ex : nano hlw.txt

|`touch`| use this command to create an empty file. |

Ex : touch hi.txt

|`mkdir`| use this command to create a directory |

Ex : mkdir newfolder

|`rmdir`| This command is used to remove empty directories. |

Ex : rmdir newfolder

|`tree`| use this command to see folder structure like tree, |

Ex : tree hlw.txt

---

# User and Permission Management

| Command | Description |

|------------|-----------------|

|`whoami`| this command Displays the currently logged-in user. |

Ex: whoami

|`id`| This command is used to see user or group ID. |

Ex: id

|`sudo`|  Run command as root (sudo = super user do) |

Ex: sudo apt upgrade 

|`chmod`| This command is used for changing file or directory permissions. |

Ex: chmod 755 script.sh

|`passwd`| Use this command to change the current user's password. |

Ex: passwd user

---

# Networking Commands

| Command | Description |

|------------|-----------------|

|`ping`| use this command to check the internet connectivity. |

Ex: ping google.com

|`ifconfig / ip a`| use this command to see the ip address  |

Ex: ifconfig

Ex: ip a 

|`netstat -tulnp`| use this command to see open port and running service. |

Ex: sudo netstat -tulnp

|`ss -tulnp`| Use this command to see open port and socket information. |

Ex: sudo ss -tulnp

|`iwconfig`| use this command to see wireless network information. |

Ex: iwconfig

|`wget/ curl`| use this command download or fetch form web |

Ex: curl http://google/com

|`nmap`| use this command to scan the network. |

Ex: nmap 192.168.1.1

|`traceroute`| use this command for trace network path. |

Ex: traceroute google.com

|`nslookup`| use this command to see the ip address of the domain. |

Ex: nslookup google.com

|`dig`| use this command to see the DNS information. |

Ex: dig google.com

---

# File Search and Manipulation

| Command | Description |

|------------|-----------------|

|`find`| use this command to search files. |

Ex: find . -name file.txt

|`locate`| use this command to quickly find any files. |

Ex: locate file.txt

|`grep`| use this command to search any specific word in files. |

Ex: grep “password” file.txt

|`stat`| use this command to see detailed information of files. |

Ex: stat file.txt

|`file`| use this command to see file type. |

Ex: file hlw.txt

|`history`| use this command to see command history. |

Ex: history | grep nmap

---

# Privilege Escalation and Enumeration

| Command | Description |

|------------|-----------------|

|`hostname`| use this command to see system hostname. |

Ex: hostname

|`sudo -l`| use this command to show which commands the user can run using sudo. |

Ex: sudo -l

|`ps aux`| use this command to see running processes. |

Ex: ps aux | grep apache

|`uname -a`| use this command to see kernel/ system information. |

Ex: uname -a

|`env`| use this command to see environment variables. |

Ex: env

|`mount`| use this command to see the Mounted Filesystem.  |

Ex: mount

---

# Tool usage and exploitation

| Command | Description |

|------------|-----------------|

|`msfconsole`| use this command to start the metasploit framework. |

Ex: msfconsole

|`hydra`| use this command for brute force tool. |

Ex: hydra -; admin -p password.txt 192.168.1.5 ssh

|`jhon`| password cracker |

Ex: jhon -rockyou.txt hashas.txt

|`nikto`| Web Server Vulnerability Scanner. |

Ex: nikto -h http://target

|`sqlmap`| SQL injection automation |

Ex: sqlmap -u “http://terget” -w wordlist.txt

|`wireshark`| packet sniffer (graphical user interface) |

Ex: wireshark

|`burpsuite`| Web Application Testing Platform (graphical user interface). |

Ex: burpsuite

|`drib / gobuster`| directory bruteforcing. |

Ex: gobuster dir -u http://terget -w wordlist.txt 
