# SAP-1-EEE-4308 Project by Team FrostByte, IUT
SAP-1 (Simple As Possible)  Architecture Based 8-Bit Computer Design Done in simulating software named "Proteus".

This is a Lab Project of EEE undergrad from a small team of Educational Institution named IUT , Bangladesh.

Member of the Team:

Mainul Islam

Wasik Billah Ibn Rashid

Sifat Aziz


![image](https://github.com/Mainul-Islam-07/SAP-1-8-Bit-Computer-Design/assets/78782260/b7795d27-1d37-492d-b5bb-20017e050311)

Problems and Corresponding Solutions (If present):

*For clock pulse generator, we were getting a fatal error message and the simulation was aborted 
when we tried run the program in automatic pulse from the starting. To solve that we used a pull 
down resistor in the output of astable mutivibrator. Still we did not get acquired result as it only 
gave stable 0 state but not 1. So we used a voltage source in the output to boost the output 
voltage level.

*In the ram we did not use the subcircuit name as accordingly so we suffered from unusual 
behavior of ram.

*In reducing the microinstruction when the input from program counter was connected with 
MAR with the bus there was clash of values, so to get acquired result we used a MUX.

*In reducing microinstruction, we also faced problems as in the first T-state from negative pulse 
to positive there is a garbage value and since the IR triggered before RAM sending desired 
output in the BUS, we got garbage instruction stored in the IR. To resolve it, we used multiple 
number(14) of NOT gates to delay the triggering and to get acquired instruction stored in the IR.

*After integrating all the components in the project we did not firstly include the output of ALU 
in the BUS. So the Accumulator after always stored garbage value which was resolved when the 
output was given.

*Despite producing the sign bit and carry bit from the ALU, the value of sign bit and carry bit 
was not being stored in the ALU. So these two bits were send directly to the accumulator and the 
output unit
