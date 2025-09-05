A brief report about the project can be found in "**8 bit computer_report**".

For this project, I took inspiration from Ben Eater's "[**8-bit computer from scratch**](https://eater.net/8bit)". While Ben demonstrates how to build the computer on a breadboard using ICs and real hardware, I implemented it in Proteus using mostly the same chips, except for few, such as ROM chips. For ROM chips, I used an alternative IC. Since the Arduino-based method for writing data in ROM was not viable in my case, I manually entererd data into each memory location and then uploaded the .hex file to ROMs.



**Specification of the 8-bit Computer:**

Clock: adjustable-speed (from less than 1Hz to a few hundred Hz). Realized up to 350Hz

RAM: Two units of (16 words × 4 bits)

ROM: (2*32KB) for Control Unit

Instructions supported (as of now): LOAD, ADD, OUT, HLT (not Turing Complete)
If we add unconditional jump, conditional jump; it would theoretically make it Turing Complete. Practically, it is still limited by memory, clock constraints.

Units: RAM, Program Counter, Memory Address Register, Instruction Register, Register A, Register B, Output Register, Clock, Arithmetic Logic Unit (Only implemented Arithmetic Instruction as of now), Control Logic Unit.


