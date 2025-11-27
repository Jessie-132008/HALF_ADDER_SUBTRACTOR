# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
module jessie(a, b, sum, carry);
input a, b;
output sum, carry;

assign sum   = a ^ b;   
assign carry = a & b;   

endmodule


module jess(a, b, diff, borrow);
input a, b;
output diff, borrow;

assign diff   = a ^ b;        
assign borrow = (~a) & b;     

endmodule
```
 Developed by:JESSIE J

 RegisterNumber:25017372

**RTL Schematic**
<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/d7f62735-92f8-4f55-9505-813022e70f13" />
<img width="1920" height="1080" alt="Screenshot (20)" src="https://github.com/user-attachments/assets/aaaf9baf-0fe7-4350-b542-2eecb08c19be" />

**Output/TIMING Waveform**
<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/7902816a-ea1d-43c8-bbd2-7d2d1c9f2d2d" />
<img width="1920" height="1080" alt="Screenshot (21)" src="https://github.com/user-attachments/assets/af4cd3ea-27e2-43dc-a874-c2597ce4fcf2" />

**Result:**

  Thus,a half adder and half subtractor circuit is designed and its truth table in Quartus using Verilog programming is verfied.
