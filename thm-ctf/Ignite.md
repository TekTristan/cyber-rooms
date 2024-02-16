ignite ctf less goo
-

1.) checked the website
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/b9a4d463-5575-4e05-8289-f35e80c6e50e)
- looked at nmap scan rq
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/e9ec97ea-b167-4916-b044-d4f257ba1705)
- shows something with robots.txt and with my past experience that would have some sort of information or clues to penetrate
- user-agent * means that all users can not have any access to a directory that has /fuel/ where it says disallow
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/cbe58dca-617f-491a-9313-98174d40c810)

2.) gobuster just in case
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/df1d6b87-d8c1-445a-ba62-3f245fa5fb83)
- robots.txt like before is open

3.) searchsploit for more clues
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/3c1a5ae2-4bb9-4ae6-9569-96e94049e31c)
- some results
- side note: possible sql injection since i have to possibly install the cms datababse
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/63dc24c2-a211-4349-9fc8-78858a6c7256)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/42149ea3-e8a4-4d32-b64f-ee8c232aa623)
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4f268aca-1e16-4a1b-9ddc-b48b0b08c85d)
- i overthought the process, just tried to use admin : admin as username and pw in /fuel and it worked 
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/6214cb9c-e3a4-4729-8616-e0ab26f1e38c)
- possible create a new user? but i already have admin with super duper privleges.
- at this point i am trialing and error
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f9fdd3cd-1a7a-4909-a833-5d36ed191b0e)

4.) found the right script
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/0fe32828-2cfa-4d3c-b889-817fdd7badb2)
- after finding the script i would move it to another file and edit it
- ![Uploading image.png…]()
- after I changed the url to the website i used netcat and ran the rm command to spawn a shell
- part 1: ![Uploading image.png…]()
- part 2: ![Uploading image.png…]()
- and got flag, and trying to spawn a nicer looking shell then privlege escalation

5.) privlege escalation
-


