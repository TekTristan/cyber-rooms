cyborg ctf, encrpyted archives
-

1.) nmap scan like a boss
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/381ef22a-bda5-4c20-a36d-83305292fad9)
- webpage
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/26b91e0b-5fb7-4560-9945-b10fb61ceed3)
- nmap scan and peeped port 22 and 80, ssh is a go.

2.) gobuster to get them directories
-
- given /admin and /etc
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/dc017a05-3aeb-4696-9f02-c014167d7848)
- download a archive file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/44049137-2e21-4039-b14f-390f03a0a031)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/86a956aa-96d2-4ade-a036-293777e48085)
- /etc has a user and password that is in a hash.
- need to check what kind of hash it is.
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5cac8aa9-5b17-4b5b-8bc6-64d151cd96db)
- MD5 hash, now i want to use john to extract it.
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/49e07a2e-5980-4975-88b2-f9955a8816ce)
- trialed and error with ssh.

3.) extract archive file.
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7fde8da2-d3e6-4b13-81e7-73b8bf4199b3)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f128f690-15f8-4420-84e4-084c3790bf70)
- installed borg now its time to extract
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e821563c-4b37-412d-8e60-eb19303050cb)
- music_archive was the archive to grab
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ba1840c1-8b9f-4f2e-9887-b429f2c6dc3d)
- new password and username for ssh.

4.) ssh into alex
- 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b0cea2e0-5d75-4b43-bc74-ef20bc0bac72)

5.) privlege escalation
-
- i have trouble with this one but we will see how it goes
- messed around and got this message
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/99fb086f-ff71-46dd-931c-651c12923879)
- so possible i can run a bash script or something inside the backup.sh to get root
- so somehow since the script has escalated privleges that I can work with and peeped getopts, i can run this?
- i am still confused on this part
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e45e4630-ab0f-44ac-a5b2-bbb3e764dcee)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d2618ab3-fc16-4da6-980c-81efdd8ae8fc)
- i wasnt able to run any commands and it wasnt showing up in the root shell so i did the command from before in alex again to change the permissions of the bit on the binary of the root shell command /bin/bash
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/1055888c-7473-4362-8bf4-2fc465fe149e)




