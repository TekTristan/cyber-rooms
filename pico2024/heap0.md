this week of new binary fweaking exploitation my brain is loaded with chicken bakes and cookies from costco
-

1.) read the source code and figure some stuff out
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4275491b-d66b-4646-b311-42531cfdd7e9)
- the printed states
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/70f3009f-a7c2-46ed-8974-9194e9c6822f)
- and basically understanding that it could be overflow
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/8e5f6c73-1da0-47e6-81a8-627d0a6558fe)
- scanf has no limit for the number of characters, and input_data is only up to 5 for the specific size and so is the safe_var
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/4f696774-232f-44d0-bd6c-d076c4da6365)
- understanding that both of the vars are allocated w/ malloc without any gaps, which would mean that they would be adjacent in memory
- to overflow from input_data to safe_var

2.) time to overflow that boy
-
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/f60cb2da-aa29-4473-91cd-d12f39aef221)
- subtracted the differences unless there is some sort of super duper way
- then provided the difference with pico at the end
- ![image](https://github.com/TekTristan/cyber-rooms/assets/92371193/bcefc5ff-eeca-458c-96a2-2968a3e56736)

