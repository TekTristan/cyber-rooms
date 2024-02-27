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

6.) 6ix crackme filessss
-
- I see that it is not stripped, and it is looking for a pw
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f0b22639-8060-4db3-843d-015d7c4a29d7)
- not able to look at it with ltrace
- using radare2 a reverse engineering tool to go deeper into the file
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a54e7a2d-1349-4993-ae98-1aa2d29f217c)
- aaa to analyze, afl to look into the function lists,
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/dfbd871c-09d3-4bd2-b615-5876e2eaf772)
- pdf @ main to open the function and look into each address
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/ebd5c2cd-57ea-4fb6-9475-2c50813255a5)
- went into securetest and see a bunch of if-else or jmps
- using s sym.my_secure_test to analyse the beginning of the function, then using VV to form a flow chart for simplify and ease the search
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d07668ae-98f0-43fe-ab1b-bcde567b75b6)
- the flow chart in HEX has it compare the password bit by bit from 31 to al and 33 to al, then putting those hex values from the top to bottom of the flowchart in cyberchef you get
- 1337_pwd

7.) doing the usual
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/bac201ce-ce45-4f96-ae53-5e9a10e8022a)
- while running this is the output giving it a user friendly need for a input
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/40d89341-6b50-4229-bdd9-8946a8635e93)
- using radare2 for this
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5fb594f7-5076-4e09-a90c-87682081f40f)
- going into the flowchart for main there is a f/t or if else statement whether the input is 1 or not 1
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/d0ca4569-2ecb-4a8e-b2ec-720aceb524ad)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/20c95571-2dbc-4cce-b90e-467ed33447e9)
- this chart is showing me a t/f if i get it false then i am a hackor so possibly this is the right way
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/1c02a268-1c0e-4fe8-b8fa-46ab5d6c98eb)
- convert from hexadecimal to decimal you get 31337
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/819a90c3-903d-473f-9438-abaf86e13597)

8.) doing the usual for number 8
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/470ab856-4911-4503-bb72-bbeb6195fb18)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/dba81362-a20e-4845-9af3-e2a4b8a9c470)
- where it needs a password
- after opening radare2 and going into the flowchart of main since there is a bunch of jmps i see this
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/677e4ae7-266b-4e71-a881-b9f89ec4f7e3)
- convert then run
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5b8c8f9d-505c-406f-be73-61da9e4a65bb)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/9aa093ce-42b3-47e2-8337-78d49501290b)
- now i am done!!!
