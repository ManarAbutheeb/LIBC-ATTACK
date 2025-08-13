# LIBC-ATTACK
CS442-ASSIGNMENT 

1. Task A
a. Environment set up: switched off stackGuard protection and address 
randomization, and turn on countermeasure, change owner to root and mod to read and write
b. Debug the program using gdb to find address of the system() and exit()

3. Task B
a. Export MYSHELL variable, and execute the code to find /bin/sh address

4. Task C
a. To find the offset distance Set the break point at bof() function then run
b. Print the address of register ebp and buffer then calculate the distance which is =282
c. The updated code:
The content loop range with 1000 because the function in retlib.c has size of 1000
Assign sh_addr with 0xbffffe1e, with range [294,298]→distance +12
Assign system_addr with 0xb7e42da0 and range between[286:290]→distance+8
Assign exit_addr with 0xb7e369d0 and range between [290:294]→distance+4
d. Execute the exploit code and vulnerable code then we got the root shel
