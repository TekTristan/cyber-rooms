the network security challenging my brain
-

1.) checked out the page and nothing special or in the page source
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3b197055-1fd4-4759-a3c3-b427139dce07)

2.) nmap scan that big boi
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/045ed50d-b2cb-4415-96e5-598535d1b656)
- see ssh is open, smb, and possible login
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8f8506f7-f3cd-422f-9eba-b3bb770aa1f1)
- the better nmap scan to show that -p- would do all ports, -T4 makes it faster, -vv is verbose so more details
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/2ee82f80-2315-4994-a13e-f9a90b32ec91)

3.) hydra not hail hydra that is weird, and i love captain america
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/39bd891a-3a8f-4152-b35c-d0ed8fe35ddb)
- given two usernames and using hydra and the open port to ftp login later
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/502c5db2-fe1a-41a7-92ae-dae2ecb806f9)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/a905845d-f75a-4cb2-8a2f-ba88f6d53837)
- time to login and find the flag

4.) ftp with them passwords that i lovely hacked and cracked and sacked
-
- wow first try that i got the right acc and flag wowwow
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8782b39a-dbc8-4e7f-a127-171fab941f5f)

5.) tcp scan with being super hidden like ninja not the fortnite streamer
-
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/85be8e98-1693-4686-8be9-8fd59adc30fb)
- only possible if you nmap scan with -sN as it pull in null packets with no flags set
- and done fun
