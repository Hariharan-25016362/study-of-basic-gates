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

 Developed by: HARIHARAN M RegisterNumber: 25016362
 module logicgates1(a, b, c);
    

input a;
    input b;
    output  [6:0] c;
	assign c[0]= a & b;
	assign c[1]= a | b;
	assign c[2]= ~(a & b);
	assign c[3]= ~(a | b);
	assign c[4]= a ^ b;
	assign c[5]= ~(a ^ b);
	assign c[6]= ~ a;

endmodule
 
**Logic symbol & Truthtable**
![WhatsApp Image 2025-12-05 at 07 54 34_78cf8138](https://github.com/user-attachments/assets/9ed779c1-56fd-48a4-b005-adb0532ef68a)


**RTL realization Output:** 
<img width="1325" height="880" alt="Screenshot 2025-11-23 202949" src="https://github.com/user-attachments/assets/3670e2e8-6ce6-4c44-a3a1-22b59b996aae" />

**RTL**
<img width="1918" height="664" alt="Screenshot 2025-11-29 124640" src="https://github.com/user-attachments/assets/3d028542-1ee5-4471-8b4f-1be32e3e80d7" />


**Result:**
Studied and verified the truth table and logic gates in Quartus II using verilog programming


