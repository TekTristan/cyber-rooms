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
