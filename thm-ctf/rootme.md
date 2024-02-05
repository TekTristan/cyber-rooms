![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b54430cb-df96-40b2-98c5-e3191ee9e345)rootme ctf yaa
-

1.) nmap scan like uszal
-
- nmap -sC -sV (iP)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/1b884232-a0b7-4c11-9e3c-53eae989017b)
- nothing special just the usual so far

2.) gobuster to bust that directoriessss!!!!
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d81403a3-50ee-4f79-8012-d2449c9e0724)
- found mulltiple directories like upload and panel that i could use

3.) while on the webpage, i could upload files and use to exploit, recently learning about php injection
- 
- created a php file with nano name.php
- didnt let me upload php files and had to learn to bypass
- at first i changed it to php.jpg but that didnt work, so i changed it to .php5
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/91ce4b4a-4c46-49fe-9327-c0340e28a55a)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e36e6070-ff7b-4f31-a413-df9e316f78e7)
- had to find the directoriy where my php injection is and run it and have netcat running on my terminal
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7323d00e-2851-491c-b7fe-6e18693c5d63)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/9e99ccc1-2ea0-4181-8240-6e3f62e1fabc)

4.) while in the shell i tried to find user.txt with locate and find normally but that didn't work
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/c21e56e3-b964-4294-b190-8bef1dee532f)
- / is the directory i am searching from, -type f is an option to only find file, and -name user.txt is the specific name i am finding, for notes
 - ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/678c9f90-21b5-4c28-bf79-3aeaea4f1b2d)
 - then got my txt

5.) privlege escalation
- 
- ran a command to find the executable commands that I have that is the same as a owner or root or SUID
- and ran this
- find / -user root -perm /4000
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e6d7f3f6-bb17-4be1-bf62-efe81a9cab55)
- where i could run some python script or something related to exploit into root and went into the hints to help and used GTFOBins 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/c8550971-cc6a-494c-946c-64075fbd772f)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/05f9020b-592d-437e-a36f-cec3734591c1)
- typed python and found my command to use 
 - ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/cfb42b3f-39f3-4d93-be97-22eed2fb6f05)
 - and basically done!

