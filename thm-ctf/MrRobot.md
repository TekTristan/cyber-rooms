taking control of robots in a ctfs
-

1.) cools pages and kinda scary
- 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d061675b-8865-4fe1-b71e-0715cf98e522)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/da9c23e1-bcec-4bbc-bdd3-fd9edf5bdf4e)
- no hints in page source

2.) nmap and gobuster
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3177f0b8-4646-4a24-924a-855147450a85)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4fc5d4ff-c2fc-4c79-a140-72c2b4db6ad4)
- alot of damn directories
- looked up /robots.txt for funzies
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/bd8efbb9-7c66-4988-96d4-00c9496d5e78)
- given the first key 
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/770ecbba-38e6-40a9-938c-a17b2f69e489)

3.) rand
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/6b99a8aa-18ab-49fd-9104-be72f84eef32)
- randomly got these usernames? or some sort of clue
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/1c89c6b8-d6a5-4cb6-9185-b35a7cc62650)

4.) used hydra for username and to find password
-
- do not want to rewrite notes so here is my onenote screenshot
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/838f1733-4648-4ec8-a9d3-639e779b69a2)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5e8721d7-7935-4888-857a-f0c86205738d)
- nice login ig

5.) messing around again
-
- since php possibly run a reverse-shell script, tried import or export something but dead end, found editor
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/966fa292-3d73-4eb3-a102-17e5b5d686de)
- wrong file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0cba2b07-46c7-4036-902d-d486202596d8)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5c7effcb-d3fc-4352-a727-73e95c726b36)
- got access and shell but cannot open the text file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/fa6e3c63-181f-486a-8919-39944ef813a0)
- clearly md5 hash
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7a005146-e577-40fc-a58a-45831523a5aa)
- so convert it to find the pw for robot
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/56f64127-8344-4b56-a424-4188bd48042e)
  - 	abcdefghijklmnopqrstuvwxyz
- after getting key 2 privlege escalate

6.) priv escalation
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e042f7be-5c59-4efe-ba81-3ab2cfd148d2)
- uh okay?
- ran a command to find suid bit set that I can use to gain root
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4d74aeb3-38b9-4491-9316-93a138eb785d)
- nmap boooiii
- look at gtfo bins
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/09a21cce-832f-4861-851c-9403d9c352d2)
- okay time to cook
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/72696b9a-7700-4d95-8a58-5acea7ca72e9)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a6e42762-edc8-474c-8d3c-d55c17a3ed41)
- doneeeeeeeee
