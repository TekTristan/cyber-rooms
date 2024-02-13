brooklynNine o Nine ctf
-

1.) looked at the webpage and source
-
- did not find anything.
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3e9b0c97-7590-43d9-8eca-19efb7425370)

2.) nmap scan 
- 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3f7fc144-55bb-4904-8d52-e16bde5d6fcc)
- i see that i am allowed with ftp and login with anonymous

3.) login with anonymous
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2a5fd3f6-a040-4600-be65-18cd7ebc4e5f)
- grabbed file and now to open
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e0263c33-7ce1-46e8-89dd-f0acd1b3045e)
- so jake has a weak password and we know that ssh is open.

4.) gobuster time
-
- nothing showed up on gobuster
- i missed something in the page source on steganography
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ab17cddd-be99-47cc-a270-79b1114c4a19)

5.) i just went and hailed mary and hoped hydra would find something and it did
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ecf3a02f-dc84-45d3-8a3d-819be1e1dd4b)
- time to login via ssh
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e0548970-d8ab-4a42-98ff-2cb9ce70967f)
- got user flag

6.) privilege escalation
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/cc1416ae-ae77-4a82-a5f0-1ed003081313)
- all no passwords in /usr/bin/less, so GTFOBins it is
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/82787b78-a603-4b83-abad-a553942a1c9c)
- bam solution
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a36af669-c276-495c-ab47-4a4c677f2936)
