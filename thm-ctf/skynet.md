skynet ctf, in progresssionnn
-
1.) viewing the website
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/57749b88-68c5-454b-940b-871484c55d64)

2.) used nmap to scan for open ports 
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5595c318-4cff-481d-ae0d-41eefc4b39d0)
- found something with SMB. used for later

3.) gobuster for them open directories
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f3ade957-23a9-44fe-86a6-a1e0e05fb132)
- this is the webpage

3.) smb into anonymous
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/7a41099b-79db-4010-a432-43b914b802c8)
- get the files.
- look at the log passwords then use hydra

4.) hydra with http-get-post 
- 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d15a663e-c11e-4f76-87ff-1a91cd49d9f8)
- log into squirrelmail wooo
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/fdd1ef66-4f86-4b73-976e-578bba290f08)
- got password for milesdyson

5.) log into milesdyson in smb
- 
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/963af30b-92a9-4cda-90e1-fdb508ca03d2)
- /milesdyson is the sharename -U for the username and milesdyson again since he has access to the sharename directory.
- grabbed the important.txt and found the cms hidden directory
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f4c3afd8-93c2-4359-ae82-118b84c495a4)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/1f92ee8e-ebab-4ee6-aa45-9761dcbd40f1)
- webpage of his personal stuff
- use gobuster again since we found a different hidden directory

6.) gobuster pt2




- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/507a778d-4f28-4a00-a2db-a440a5485ccb)

