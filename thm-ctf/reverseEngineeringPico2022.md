picoCTF 2022 of the Reversal of the Engineering of the brain
-

1.) file-run 1
-
- used file to go deeper into details, change permissions of file, then boom
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/61e18e07-ceae-48b1-aae0-479ac7729aa1)

2.) file-run 2
-
- ran file, then tried to execute the program, changed privleges, and it said to have one argument when running, then said I had to use Hello! while running, then BAM!
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/86b1cd35-48fb-4549-a07a-fd330cc82f6c)

3.) GDB Test Drive
-
- tried to run gdbme and it had no output, changed permissions of gdbme file with chmod (chmod 777 file) to change fiel permission to give read write and execute to the owner.
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/c38b4913-87d6-4d0d-88d8-70ef9304b1a9)
-![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8d4b1c7d-893a-4e48-a891-85190532f800)
- layout asm to show the assembly code with each register, saw how it used call with sleep function, moved the breakpoint there with break *(main+99) then jmped over the breakpoint to not run sleep then the flag ran.
