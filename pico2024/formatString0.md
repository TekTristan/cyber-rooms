fun binary exploitation as a noob

1.) looking at the c source code 
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/150443ee-12f7-4a3b-b07a-3da0c0795a39)
- serve_bob() function is only turns on once we have a input that is 2 times the length of buffsize, which is 32
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/cf41b0cc-662a-4242-a03e-577a72eee83a)
- - so based on my understanding Gr%114d_Cheese, the %114d specifiert is asking for that tells the printf to print an integer that is at least 114 characters wide,
- and since there was no integer provided, it used garbage values.

2.) getting the flag is 
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/5f1ffec0-80c2-43c1-9eca-2e71e8c9d0bb)
- based on thsi snipped we want to execute a segmentation error that we can provide with printf
- Cla%sic_Che%s%steak was the option for spongebob and was the seg error since %s was a misuse of the format string which could trigger a seg error.
