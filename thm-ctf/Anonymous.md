anoymous like the lizard squaaaad
-

1.) nmap scan my lizard 
-
- ran this  nmap -sC -sV -p- -T4 --min-rate=9326 -vv 10.10.219.255
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/061873de-ba3d-4350-90f6-33125d3e424a)
- ftp is open with smb
- files that i got from ftp
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3a3e83b4-81cb-4df5-a2ac-db3153f22be4)
- smb shows these sharenames
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/21ef5813-3ba4-403e-b56c-f93af1565a4d)
- break time, imma go hoop to cool off a bit

2.) look at smb
-
- got the pics
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/044ded74-4dd0-4794-8b01-045191c2024b)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/914fc7c9-cb4f-4fac-ab1c-186007c7bc61)
- tried to use steghide but that was a deadend
  
3.) edit the clean.sh
-
- after getting the clean.sh file and looking at it, edit the file to put a bash-script in it, since it is ran
- bash script from pentest monkey
- chmod +x clean.sh to change permissions to executable then send it back up to ftp
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/48c40fb2-4a5d-465b-a392-da196303184d)
- ran a nc listenter on another tab then got my user.txt file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/6e6c6bc9-2008-4452-8a0d-ceaf77d9fb7f)

4.) privilege escalation
-
- transferred over the loud ass linpeas
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/33e3b158-179a-479a-bb5c-be522342a584)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e2259648-4da4-41f0-83fa-8abb33f1c0e9)
- python server first of course
- then giving it executables with chmod ran it
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/dd83abdc-4cb8-457e-a623-1dc4416d4658)
- looked at gtfo bins for that w
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/bd544e00-f9b7-44f8-ba9a-0b2f300d2bbb)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/14581abb-adf9-4afd-9023-0eb74496655e)
- badabing badaboom done 
