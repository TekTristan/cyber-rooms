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


