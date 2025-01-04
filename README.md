### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**

Program for logic gates and verify its truth table in quartus using Verilog programming
'''
module exp1de(a,b,c,d,e,x,y,z);
input a,b;
output c,d,e,x,y,z;
assign c = a&b; //and gate
assign d = a|b; //or gate
assign e = a^b; 
assign x = ~(a&b);
assign y =~(a|b);
assign z = ~(a^b);
endmodule
'''
 Developed by:Prathiksha.R RegisterNumber:24900337 
 
**Logic symbol & Truthtable**

![Screenshot 2024-12-17 132752](https://github.com/user-attachments/assets/232cd131-02eb-4b58-90a5-df7842bb1894)



**RTL **

![Screenshot 2024-12-17 132808](https://github.com/user-attachments/assets/72317d0a-4269-4be2-b2e3-5feb86902f8d)



**RTL realization Output:** 

![Screenshot 2024-12-17 132803](https://github.com/user-attachments/assets/9b748477-27e7-4652-92b2-a9012391da10)

**Result:**

The truth table of the specified logic gates(AND, OR, NOT, NAND, NOR, XOR, XNOR) was successfully implemented and verify using Verilog programming in Quartus II.


