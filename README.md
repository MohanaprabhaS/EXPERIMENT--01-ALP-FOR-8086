# EXPERIMENT--01-ALP-FOR-8086
# Name : Mohanaprabha S
# Roll no : 212224040197

## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```

## Output  

<img width="1155" height="689" alt="image" src="https://github.com/user-attachments/assets/9376ca51-59a7-469e-aad4-fba8a57cf4d4" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
 
## Output  

<img width="1159" height="688" alt="image" src="https://github.com/user-attachments/assets/51f0b1cd-c73c-4399-8ad8-a4b66db8f053" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  

 <img width="1152" height="681" alt="image" src="https://github.com/user-attachments/assets/e518c86c-7871-4bc1-85ce-0d8444cd5a4e" />



## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```


## Output  

<img width="1163" height="694" alt="image" src="https://github.com/user-attachments/assets/a5b9de66-ac98-436f-a892-8c6d2ad141be" />

## Programs for logical operations
## AND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

## Output

<img width="1161" height="691" alt="image" src="https://github.com/user-attachments/assets/83a3031a-0ae7-47a2-8eee-ce339cd3b794" />


## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```

## Output

<img width="1162" height="691" alt="image" src="https://github.com/user-attachments/assets/712bcf13-e754-43bf-8bd9-9618d87b7918" />


## NAND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output

<img width="1155" height="688" alt="image" src="https://github.com/user-attachments/assets/093d1749-a473-4fd0-bfcc-afe523a50b5e" />


## NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output

<img width="1157" height="685" alt="image" src="https://github.com/user-attachments/assets/42d1d392-6f1e-41e8-ab50-fd90101214db" />


## NOT
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```
## Output

<img width="1157" height="688" alt="image" src="https://github.com/user-attachments/assets/e9639290-c548-473e-8931-7bc97610338a" />


## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```


## Output

<img width="1157" height="687" alt="image" src="https://github.com/user-attachments/assets/2c0f1b24-4f6a-47d5-965b-d37a326d0b44" />


## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output

<img width="1162" height="681" alt="image" src="https://github.com/user-attachments/assets/bea02427-d5ce-4caf-9996-0bfeaf46436a" />


## Result :

We have executed ALP on fundamental arithmetic and logical operations successfully!!!
 








