spooky tom ctf!!!
-

1.) nmapper to scatter and be a hacker
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5809e304-364e-458c-bc31-3d231df157a9)
- i can see that port 8000 is open with ajp13 as a service, but i do not know what that means. will look into it
- port 53 is open with tcpwrapped, another thing ill look into.

2.) gobuster for the custard
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/20375b49-26ef-4a3a-89e3-de04a362b30a)
- ok what the frick i skipped checking on the ports so possibly this has something to do with it.

- ajp13 is supposed to be better performance over the HTTP protocol running over tcp
- tcpwrapped is adding another layer between client and server.
- the webpage is not loading either, so maybe it has been messed with already.
- i looked online but went with using searchsploit after to possibly make it easier for an exploit
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0d85f0b1-535e-4a04-b32e-0e90d2466115)
- use this to exploit ajp13 https://github.com/00theway/Ghostcat-CNVD-2020-10487?tab=readme-ov-file
