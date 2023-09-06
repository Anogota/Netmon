1. What is the name of the application running on port 80? Given the three words in the logo.
First i did some recon, to recognaiz what's is happing on this server here is there result of nmap -sCV <IP>

![obraz](https://github.com/Anogota/Netmon/assets/143951834/eb4ca190-6559-4d45-9207-ec40265911b4)

2.What service is running on TCP port 21?
Is ftp, but when i look again on scan, we see there Anonymous, we can login to ftp by anonymous with any creds, also we see there many directory, lest check this out :P

![obraz](https://github.com/Anogota/Netmon/assets/143951834/54173928-5dff-4506-96aa-1e7ed5c181dc)

3.Submit the flag located on the Public user's desktop.
Okay let's go ftp by this command: ftp <ip> than asking as for a user, here write Anonymous and press enter, after this we they asking as about the password, press enter when we login as Anonymous we don't need a password. Track to the /Users/Public and here is the flag, but we can't use command cat to show this flag, we need to download this flag using get user.txt, here is the flag:

![obraz](https://github.com/Anogota/Netmon/assets/143951834/310fc260-0d39-4d7a-adde-9dce79106673)

4.What is the full path of the folder where PRTG Network Monitor saves its configuration files by default?
I don't know there answer, but when you copy paste this question to google, u will be see the answer, here is the answer:

![obraz](https://github.com/Anogota/Netmon/assets/143951834/dd53e497-04ce-49db-9092-b30ec5b2bf5a)

5.What is the name of the backup config file?
Little searching and i found, this file is PRTG Configuration.old.bak in directory Remote directory: /programdata/Paessler/PRTG Network Monitor
6.What was the prtgadmin user's password according to that file?
We need to download this file and check what's inside there: get PRTG Configuration.old.bak, when u download this and cat, u can see many lines of code, we need to find some creds
Holy shit, that was hard, there is hundreds lines of code but i found here is the password:![obraz](https://github.com/Anogota/Netmon/assets/143951834/fd1fbe6b-51c0-4a6e-9d9a-4971cb1a849e)

6.What is the prtgadmin user's password on the website now?

