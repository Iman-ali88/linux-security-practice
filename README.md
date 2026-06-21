Bandit Level 0

![Picture1](Picture1.png)

Bandit Level 0 → Level 1

Goal: Login to the Bandit server using SSH.

Command :ssh bandit0@bandit.labs.overthewire.org -p 2220

Skills learned:

·       SSH connection

·       Remote server access

![Picture2](Picture2.png)

Bandit Level 1 → Level 2

Goal: Read a file named "-" (special filename).

Command: cat ./-

Skills learned: Handling special filenames

![Picture3](Picture3.png)

Bandit Level 2 → Level 3

Goal: Read a file with spaces in its name.

Command: cat "spaces in this filename"

Skills learned: Escaping spaces in filenames

![Picture4](Picture4.png)

Bandit Level 3 → Level 4

Goal: Find a hidden file.

Command:

·       ls -a

·       cat .hidden

Skills learned: Hidden files in Linux

![Picture5](Picture5.png)

Bandit Level 4 → Level 5

Goal: Find the human readable file.

Command: file ./*

Skills learned: Identifying file types

![Picture6](Picture6.png)

Bandit Level 5 → Level 6

Goal: Find a file with specific size and permissions.

Command: find . -type f -size 1033c ! -executable

Skills learned: Using the find command

![Picture7](Picture7.png)

![Picture8](Picture8.png)

Bandit Level 6 → Level 7

Goal: Find a file owned by specific user and group.

Command: find / -user bandit7 -group bandit6 2>/dev/null

Skills learned:Searching system-wide files

![Picture9](Picture9.png)

Bandit Level 7 → Level 8

Goal: Find the line containing the word "millionth".

Command: grep millionth data.txt

Skills learned: Text searching with grep

![Picture10](Picture10.png)

Bandit Level 8 → Level 9

Goal: Find the unique line.

Command: sort data.txt | uniq -u

Skills learned: Sorting and filtering text

![Picture11](Picture11.png)

Bandit Level 9 → Level 10

Goal:Extract readable strings.

Command: strings data.txt | grep ===

Skills learned: Extracting readable strings

![Picture12](Picture12.png)

Bandit Level 10 → Level 11

Goal: Decode base64 data.  
Command: base64 -d data.txt  
Skills learned: Base64 decoding

![Picture13](Picture13.png)

Bandit Level 11 → Level 12

Goal: Decode ROT13 text.  
command: tr  
Skills learned: Simple cipher decoding

![Picture14](Picture14.png)

Bandit Level 12 → Level 13

Goal:Extract data from multiple compressed files.

Commands:

·       xxd

·       gzip

·       bzip2

·       tar

Skills learned:

·       File extraction

·       Compression formats

![Picture15](Picture15.png)

![Picture16|517](Picture16.png)  

![Picture17](Picture17.png)  

![Picture18](Picture18.png)

Bandit Level 13 → Level 14

Goal: Use private SSH key to login.  
Command: ssh -i sshkey.private bandit14@localhost -p 2220  
Skills learned: SSH key authentication

![Picture19](Picture19.png)  

![Picture20](Picture20.png)  

![Picture21](Picture21.png)  

![Picture22](Picture22.png)

Bandit Level 14 → Level 15

Goal: Send password to a port.  
Command: nc localhost 30000  
Skills learned: Using netcat

![Picture23](Picture23.png)

Bandit Level 15 → Level 16

Goal: Connect using SSL.  
Command: openssl s_client -connect localhost:30001  
Skills learned: SSL connections

![Picture24](Picture24.png)  

![Picture25](Picture25.png)

Bandit Level 16 → Level 17

Goal: Scan open ports.  
Command: nmap -p 31000-32000 localhost  
Skills learned: Port scanning

![Picture26](Picture26.png)  

![Picture27](Picture27.png)  

![Picture28](Picture28.png)  

![Picture29](Picture29.png)  

![Picture30](Picture30.png)

Bandit Level 17 → Level 18

Goal: Find difference between files.  
Command: diff passwords.old passwords.new  
Skills learned: Comparing files

![Picture30](Picture30.png)  

![Picture31](Picture31.png)

Bandit Level 18 → Level 19

Goal: Execute command despite restricted shell.  
Command: ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme  
Skills learned: Running remote commands

![Picture32](Picture32.png)

Bandit Level 19 → Level 20

Goal: Use setuid program.  
Command: ./bandit20-do cat /etc/bandit_pass/bandit20  
Skills learned: Privilege escalation basics

![Picture33](Picture33.png)

Bandit Level 20 → Level 21

Goal: Use netcat listener.  
Commands: nc -lvp port  
Skills learned: Network communication

![Picture35](Picture35.png)

Bandit Level 21 → Level 22

Goal: Read cron job script.  
Command: cat /etc/cron.d/...  
Skills learned: Cron jobs analysis

![Picture36](Picture36.png)  

![Picture37](Picture37.png)

Bandit Level 22 → Level 23

Goal: Read cron job script.  
Command: cat /etc/cron.d/cronjob_bandit23  
Skills learned: Cron jobs analysis

![Picture38](Picture38.png)

Bandit Level 23 → Level 24

Goal: Read cron job script location.  
Command: cat /usr/bin/cronjob_bandit23.sh  
Skills learned: Script analysis

![Picture39](Picture39.png)

mkdir /tmp/iman99999

chmod 777 /tmp/iman99999

cd /tmp/iman99999

![Picture40](Picture40.png)

#!/bin/bash  
cat /etc/bandit_pass/bandit24 > /tmp/gameplan1/password

![Picture41](Picture41.png)  

![Picture42](Picture42.png)

Bandit Level 24 → Level 25

Goal: Brute force the PIN code.  
Command: nc localhost 30002  
Skills learned: Brute force basics

Cd /tmp/iman99999

nano brute.sh

![Picture43](Picture43.png)

chmod +x brute.sh

![Picture44](Picture44.png)  

![Picture45](Picture45.png)

Bandit Level 25 → Level 26

Goal: Escape restricted shell.  
Command: v (inside more → opens vim)  
Skills learned: Shell escape

![Picture46](Picture46.png)  

![Picture47](Picture47.png)  

![Picture48](Picture48.png)  

![Picture49](Picture49.png)  

![Picture50](Picture50.png)

Bandit Level 26 → Level 27

Goal: Spawn a shell from vim.  
Command: :shell  
Skills learned: Vim shell access

![Picture51](Picture51.png)  

![Picture52](Picture52.png)

Press v to inters vim text editor mode

![Picture53](Picture53.png)

Enter

![Picture54](Picture54.png)

Password level 26:

![Picture55](Picture55.png)

Enter again

:set shell=/bin/bash

![Picture56](Picture56.png)

shell

![Picture57](Picture57.png)  

![Picture58](Picture58.png)

Ls -la

![Picture59](Picture59.png)  

![Picture60](Picture60.png)