I am too lazy to open my kali machine to show this, so this is based off the webshell on pico

1.) download the files
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/6946fa60-b48c-4650-bdaa-e4cc3593e0b3)
- w/ wget lol
- unzip challenge.zip

2.) check them fles out
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a3527be0-1cdf-4c6c-acef-d624341fa6e8)
- seems like someone messed it up ig
- but the challenge is asking who was the user that could of messed up the file
- so with some git knowledge
- after running git log
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8d5db314-2edc-4060-ba83-d7b9cdb965b4)

3.) final answer
-
- use this to check for all users includign all unique authors
- git log --all --format='%aN' | sort -u
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/bf096916-4bcf-45b2-8c5d-ad7a67409c94)

