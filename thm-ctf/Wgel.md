the w of the gels ctf
-

1.) checking the page
-
- looks like nothing special so far
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4d621b8c-871f-43fd-a775-b7e329268238)

2.) nmap scanning boooooo
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/62e81c01-7a6e-43fa-aec3-4b1ded4e8fa4)
- ssh is open http is open
- clue 1 ssh

3.) gobuster for them hidden dirsss
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/c3bc526f-6a5b-4557-a555-1a8b31456f0c)
- sitemapp shows this
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0b1e607e-889f-45bb-b347-98cda26f2a3e)
- used gobuster again to get another directory for the rsa key
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/fb91f471-a3b2-40b8-9b0f-83fe03d6aeba)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/30e16b13-a4f7-4624-b331-b1f39737e562)
- if i remember correctly, i would use john to crack it

4.) john to break
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/83f919de-17bc-4bd4-a200-a4cb18e52a4d)
- uhm ok?
- i missed this clue
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d40f9b39-4dc7-49e0-9551-4b33386c9c90)
- so posssibly after changing the permissions of the rsa key then try to ssh into with jessie since it has no passphrase
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/06dc53b9-55b2-445a-807e-c628d1e2d477)
- ssh
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e223dcbb-8e8f-40ce-b4fa-a6845f5474c1)
- trial and error and im here great!!!!

5.) find flag then privilege escalation
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ee9d5a75-9467-4dbc-ab72-d8f07f3b61e6)
- time to get root
- gtfobins
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8745441d-40bd-4a38-9ce5-42ca5feb85d2)
- run a command in the exploited user
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/89f68de6-be1c-4bfe-b80f-cc2ed43fca32)
- have nc listener open first
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3b38a0df-061a-4b15-b835-0c49a4ad05a6)
- not really into shell so research after
