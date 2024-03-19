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
module exp3(a,b,cy,sm,df,bo);<br>
input a,b;<br>
output cy,sm,df,bo;<br>
xor(sm,a,b);<br>
and(cy,a,b);<br>
xor(df,a,b);<br>
and(bo,~a,b);<br>
endmodule<br>

Developed by:Vineela Shaik<br>
RegisterNumber:212223040243<br>
*/
![Screenshot 2024-03-19 083659](https://github.com/VineelaShaik/HALF_ADDER_SUBTRACTOR/assets/144340862/11447190-fb93-472b-b088-0a74698170a0)

**RTL Schematic**<br>
![Screenshot 2024-03-19 083650](https://github.com/VineelaShaik/HALF_ADDER_SUBTRACTOR/assets/144340862/30d3f0a8-d2fa-4656-ab7d-ececa69a7949)
<br>
**Output/TIMING Waveform**

<br>
![Screenshot 2024-03-19 084805](https://github.com/VineelaShaik/HALF_ADDER_SUBTRACTOR/assets/144340862/43b764a9-6586-4e14-ae4f-9fba38a80f9f)
**Result:**
 Implementation of Half-Adder and Half-Subtractor circuit was successfully verified.
