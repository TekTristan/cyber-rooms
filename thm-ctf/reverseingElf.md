easy reverse-engineering type beat s/o uzui 
-

1.) cracking the first file
-
- downloaded it and used file to find the specifics of the unknown file type
- then used chmod +x filename to change the permissions of the file to add executable permissions
- then flag
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/872ae72a-f38e-4903-84f0-5f0abcc3c5d4)

2.) cracking the second file
-
- tried to do the same thing as the first file
- then after running ./crackme2, i saw that it requires a password to open
- tried to change permissions didn't work
- used strings to look deeper or find any clues, then found the pw
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b6292f95-f0dd-4a2f-9494-81a81cfd862f)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a2a63f8f-de7b-44e6-88ad-0b687be935d5)

3.) cracking the third file
-
- just base64 so that was easy
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/faba4d3e-57f5-484c-a9eb-0588c9cdc2da)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/964b3bab-c2fa-49b8-9ca9-5e5a2f7aab72)

4.) crack the fourth of the 4th and the furth file
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/150084f8-aef7-4949-8227-e42a17739447)
- possibly means that it has some debugging information when it says not stripped
- strcmp or string compare when tried to run
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d4f5340f-23ad-4db8-8cb4-20443b33d693)
- new pw, shows that strcmp is being called with "my_m0r3_s3cur3_pwd" as one of the arguments

5.) the 5th of the cracked files
-
- file that boy
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e261eb15-989f-487b-9b73-c620957d5c89)
- again not stripped
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b10d26f3-5b1e-4084-a4ae-3b899d27bfbc)
- same thing with perms
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ba4aa67e-9f3b-48b5-b369-af7c23f90a78)
- changed perms of file and shows to enter input after running.
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/434a1359-ac33-4012-ac8d-dc6e021a7bd5)
- shows a repeatable function from anotrher input that I injected
- OfdlDSA|3tXb32~X3tX@sX`4tXtz which is the password in there, almost looked over it lol
