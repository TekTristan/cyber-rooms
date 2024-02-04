![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a9a5b60e-f867-4c8d-aa7a-c01f70cdbe1c)the laziest admin writeup for meh
-

1.) nmap scan for open ports, just always the first step
-
2.) gobuster to find open directories, found that /content was open
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2204c344-9899-4b4d-b2a2-a211af52f006)
- after looking at the webpage i did a searchsploit for sweetrice
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/697ab3a6-2bdf-41f8-8d62-d1783d6de3dd)
- really didnt know what to do with this, felt like this could used later

3.) did another gobuster scan but with /content and found a lot more directories
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4caddc93-13c8-4e8f-8a01-ec76c15c098d)
- skimmed thru the directories and found a sql backup 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/99e9a92b-7937-48cf-b94e-a64d88f70f74)
- after opening the file and skimmed thru found some clues for usename and password where the password was encrypted md5 hash
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/75498b53-44eb-45d0-ac98-04552910e592)

4.) used some online decrypter, want to use the terminal in the future, but now i needed to find the login page.
-
- went back to my gobuster scan to find the other directories and checked them out
- /content/as was the login page
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/59dc7017-6175-4588-a3d3-a7eebaaa6c40)
- at this point i went back to searchsploit to figure out what new vuln and exploits to use, then used php injection since that is something havent done or learned yet.

5.) using something from Pentest Monkey and editing the ip address and port linked here: https://github.com/pentestmonkey/php-reverse-shell/blob/master/php-reverse-shell.php
-
- where you had the searchsploit file said to use the ad section and php inject and curl to interact and retrieve the data from the url
- needed netcat on the port i chose and curl to get access
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/995a41e7-105b-4371-845f-6a162175430f)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/310d9dc9-b688-4f6e-9e3e-6c4223ca93aa)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/44098c91-3736-4663-a4a3-f7ee213451b1)
- first flag
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/939c8a99-d022-402d-a3e0-4287d4b1cca3)

6.) privlege escalation
-
- tried to sudo -l and had this clue for it 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b3cd125b-9a98-4ba3-a7c6-6e3365f0662e)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/fbcfaee5-1fbf-408e-bb04-aa65f8e78f50)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2c901ed6-4fd7-44c0-aa62-08a447db8e40)
- read and write access with /etc/copy.sh but was not able to write on it with any commandssd, and learned that you can use echo for this
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ed34251e-82b1-42e4-92f8-1ff600d2a1b0)
- use netcat first then ran sudo .... to get into root 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f56a3fcf-f101-4c01-a001-07f6392b801f)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/624238ac-c184-4f26-9623-6255df0e89e1)

7.) found root text
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f27f7fa8-9aeb-4198-ae37-a1d5d6f78144)







