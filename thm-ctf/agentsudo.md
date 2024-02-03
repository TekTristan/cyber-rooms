agent sudo ctf woooo
- 
1.) the usual nmap scan to find open ports 
-
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3ee387f0-943d-40b4-87a9-fd4f83474517)
- there were 3 open ports 21, 22, 80
- on the webpage given that codename is our username
- didnt have much with gobsuter

2.) used curl to find any connectvity to a server especially with the hint on the webpage or R being a user.
-
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a858afc6-6af5-4bb0-a9f4-0ceeb0de6436)
- -L is used for any reedirects
- A "letter" is used to inform the server about the client requesting the resource.

3.) after that since i saw that ftp port was open, and i found that chris could be a user or a codename, i decided to use hydra to find a password
-
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/adf07325-ac10-4466-837e-af0c298dab61)
- then log in via ftp
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/85586ed0-bc72-43d9-864b-020fe3d5dae3)
- grabbed txt files and png/jpg

4.) investigated further with the other files with binwalk
-
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/44812089-184d-43ad-9299-6399ac5378b5)
- received a extracted file that was encrypted so i used john to help with that 
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/69ebc65b-493f-473b-bae4-a80f9c47c736)
- after given a password and a opened the extracted file, i received something in base6 4 and easily converted it to try and open the next jpg file
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7f010fbf-a221-407f-be32-f9de0ef8797a)
- used steghide to find any other data hidden in the jpg file
- then extracted it 
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d2438504-0bdf-485e-8998-bbb77b721f13)
- was given a new user and password
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/43db714f-6c00-4842-803b-937fc4296876)

5.) ssh into the new user 
-
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d4d51b1a-39dc-4178-bde7-ff89d9908a44)
- grabbed user flag and found another jpg file.
- used scp to copy over the jpg file to use some website to find where it's from
- hint was the foxnews website
![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7f3df5cf-0799-4064-90a6-bd05639af2f3)

6.) privlege escalation with /bin/bash 
-
- looked up what to use to get into root
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/647183cd-9065-4433-96e7-335aea5e3b52)
- nice



