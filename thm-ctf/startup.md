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
