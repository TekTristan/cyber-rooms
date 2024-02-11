spooky tom ctf!!!
-

1.) nmapper to scatter and be a hacker
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5809e304-364e-458c-bc31-3d231df157a9)
- i can see that port 8000 is open with ajp13 as a service, but i do not know what that means. will look into it
- port 53 is open with tcpwrapped, another thing ill look into.

2.) gobuster for the custard
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/20375b49-26ef-4a3a-89e3-de04a362b30a)
- ok what the frick i skipped checking on the ports so possibly this has something to do with it.

- ajp13 is supposed to be better performance over the HTTP protocol running over tcp
- tcpwrapped is adding another layer between client and server.
- the webpage is not loading either, so maybe it has been messed with already.
- i looked online but went with using searchsploit after to possibly make it easier for an exploit
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0d85f0b1-535e-4a04-b32e-0e90d2466115)
- use this to exploit ajp13 https://github.com/00theway/Ghostcat-CNVD-2020-10487?tab=readme-ov-file

3.) using ajpshooter
-
- downloaded from the repo then used this command
- python3 ajpShooter.py http://10.10.98.30:8080/ 8009 /WEB-INF/web.xml read 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0cf65e4a-d5a6-408d-a934-489b699a520b)
- i assume the username and the password is at the bottom,
- using hash-identifier if its a hash
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/46ce85ba-7c60-4696-81f4-e23040dd2da8)
- no results, so maybe thats the password so ssh into it since its open
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/738cfb24-e41e-448f-97e9-f8bdf125b9d1)
- and doesnt work
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/caa4b64f-bce6-4148-ba52-b2b295b2d3ad)
- i made a mistake misspelling the username lol.

4.) messsng around
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/9b37c0eb-ccbb-4aeb-addb-0e5b066b0205)
- the credential is encrypted but the tryhackme file has a pgp private key, and i dont know what that is so research time.
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/308eea32-fd60-482e-b8f5-0248f60f10a0)
- possibly something
- got flag
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d282699f-d0c4-4400-95fc-01ed81e67fdc)
- get does not work so i am stumped
- scp is something that i saw
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ed13e012-b7c5-4727-9f7c-f21d479dea73)
- /* is all the files on that directory from ssh, /. is my local directory.
- using john to extract hash, then cracking password, gpgjohn for encrypt/decrypt, john cracking pw
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/68252171-13c4-4a04-b8b1-3ee9a727e913)
- imported key back into thm then decrypt the file to find credentials for merlin
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5b3cbd49-d99f-4840-82d1-2bde739dfa20)

5.) root
-
- use gtfo bins lol
