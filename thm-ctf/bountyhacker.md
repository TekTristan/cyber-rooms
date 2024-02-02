bountyhacker writeup
  - 

1.) nmap scan to find open ports 
  - 
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/54099765-98d6-4e35-a8af-53501210a5aa)
  - given ftp and anonymous, plus files to grab

2.) gobuster to find hidden directories just in case
  -
  
3.) login ftp as anonymous and grabbed task.txt and locks.txt
  -
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/873556c0-7ed1-47ee-a8a0-0a21d104ab0d)

4.) after getting the txt files and opening them we have the user who created the list 
  -
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/08667cbe-3de4-439f-b05e-aa8dc1a4e063)

5.) used hydra to find password for lin 
  -
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d24ea343-bf74-49d6-bdee-3c0c5d4e0665)

6.) ssh into lin
  -
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/52a68029-3e5b-401d-8964-a9e0d24e4c1c)
  - after I found users.txt and tried to sudo -l into root
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8eb1968a-fac3-4c96-b0bd-398fc66280ce)
  - since we saw tar as a clue we could sudo with this command
    -   sudo tar -cf /dev/null /dev/null --checkpoint=1 --checkpoint-action=exec=/bin/sh
7.) once we got into root or thought i did, i used whoami to doublecheck if i was root
  - then used locate root.txt to find the directory for the txt file.
      - then finally got the root.txt file 
  ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/61453ee8-3f57-4f36-89c0-557583e8350d)



