CPU
----
Transport-Triggered Architecture, Harvard architecture

How wide are instructions?
--------------------------
16 bits

Decoder Bit level pattern
-------------------------
fedcba9876543210
aaaaaaaabbbbbbbb MOV RAM[a], RAM[b]

RAM
----
First 32 addresses correspond to ALU, PC ops

Instruction Set
---------------
Memory mapped to operations

000 -> Constant 0
001 -> Constant 1
010 -> ADD[0]
011 -> ADD[1]
100 -> ADD[0] + ADD[1]

Example Code
------------
0180 MOV Constant 1, RAM[80]
8002 MOV RAM[80], ADD[0]
8003 MOV RAM[80], ADD[1]
0480 MOV Result, RAM[80]
