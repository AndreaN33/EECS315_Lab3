# EECS315 Lab 3 Report
**Andrea Norris** (adn33@case.edu)
## Introduction 

The purpose of this lab is to simulate both a sequential circuit and a 4x4 Multiplier using Design Architect IC


## Problem 1

Problem 1 focused on designing a registered combinational circuit to practice timing analysis on. We were expected to use the worst case rise and fall times for each of the gates from lab 2 to compute the longest sensitizable in the circuit. To construct this schematic, I used Nand, Nor, and Inverter gates constructed in lab 2, as well as a remade D Flip-Flop. An image of the final schematic is attached below.
 
![photo](SequentialCircuit_Schematic.png)

Some difficulties were had in constructing this schematic. Due to the nature of the lab computer's file systems, the D Flip-Flop file from Lab 2 was lost. I ultimately used one of the premade D Flip-Flops provided by the program. In addition, an OAI was needed to complete this schematic, which I did not have since Lab 2 had us create an AOI. Again, I used the provided OR gates to complete the schematic as shown. 


Waveform generation failed, as over 200 errors were generated. The errors stated that the gates provided by the program were not defined. I worked with many of my classmates in an attempt to resolve this error but we were unsuccessful.  

The critical path for this circuit would be the path with the most gates to traverse, as each gate would have similar time delays, with the exception of inverters which are less. The longest path would be through the following gates: A, C, D/E, G, H, J. 

Clock time cycle:

Setup/Hold time violations:

## Problem 2
This problem had me design a 4x4 multiplier using the shift add structure given. To complete this task, I had to create many schematics. The entire schematic is attached below, with following closeups of individual parts.

![image](4x4_Multiplier.png)

The first schematic that had to be created was the 4 bit parallel in - parallel out registers. The schematic was created as follows, using D Flip-Flops from the program:

![image](4bit_reg.png)

The next schematic that had to be created was the 4 bit adder. I made a Ripple Carry Adder, composed of Full Adder modules that were in turn composed of Half Adder modules. The breakdown of each of these schematics is below.

Half Adder:
![image](half_adder.png)

Full Adder:
![image](full_adder.png)

4-bit Adder:
![image](4bit_adder.png)

All gates used were from the DA-IC's libraries.

The final schematic that had to be created was the 2-1 Multiplexer. It's schematic is below.

![image](mux.png)

The overall schematic can be viewed more closely in the following two images.

![image](Mult_Mux_Closeup.png)
![image](Mult_adder_closeup.png)

Again, difficulties were had in generating waveforms for the 4x4 Multiplier, due to lack of definition of gates provided in the program libraries. These errors were not resolved despite the efforts of multiple students. 

Critical path:

Critical path delay:

Setup/Hold time violation:

Is the time cycle optimal?

 


