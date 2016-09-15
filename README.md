# X86
Simplified version of the X86 processor built in Logisim
32 bit processor with 8 registers and 24 address bit width RAM ~16.8MB.

Implemented a Harvard architecture using only one RAM unit but appears as a Von Neumann architecture with instruction memory and data memory being stored in two different spots. 

Possesses Kernal Mode.
Possesses TTY output screen. 

Important Addresses:
0x00FFFE00  KBSR: KeyBoard Status Register, 0 is no information is stored, 1 if there is
0X00FFFE04  KBDR: KeyBoard Data Register, stores the ASCII value from keyboard input
0x00FFFE08  DSR: Display Status Register, 0 if display is not ready for a new character, 1 if it is. Only used in slow processors. Tied to 1 in this case. 
0x00FFFE0C  DDR: Display Data Register, stores the ASCII value of the character to be displayed. 

Outstanding issues:
Need to test to make sure that it still works after I uploaded it.

To do:
Upload some binaries such as "Hello world."
Upload my instructions spreadsheet
Upload C programs that convert spreadsheets to hex
Write README.md
Write datapath
Explain what the shims do
List the commands possible

Expansion:
Could add a keyboard input
