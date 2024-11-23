# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**
Done by:A.yogesh kumar

register no:24003226
 */

 **FULL ADDER**
 
 module fa(a,b,cin,sum,carry);
 
input a,b,cin;

output sum,carry;

assign sum=( (a ^ b)^cin);

assign carry= ( (a & b)| ( cin &(a ^ b )));

endmodule


 **FULL SUBTRATOR**
 
 module FULLSUBTRACTOR(a,b,bin,difference,borrow);
 
input a,b,bin;

output difference,borrow;

assign difference= ( (a ^ b)^bin);

assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));

endmodule




/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**

**FULL ADDER**

![Screenshot 2024-11-23 110121](https://github.com/user-attachments/assets/0c90e53c-3e7c-4196-83af-d09e3dd58b7b)

**FULL SUBTRATOR**

![Screenshot 2024-11-23 110840](https://github.com/user-attachments/assets/b92ff9a7-6c0d-4239-80b7-04ed291d8492)



**Output Timing Waveform**

**FULL ADDER**

![Screenshot 2024-11-23 110520](https://github.com/user-attachments/assets/39e3648a-9300-4b57-bdad-1828fecfb4eb)

**FULL SUBTRATOR**

![Screenshot 2024-11-23 110933](https://github.com/user-attachments/assets/7530c85f-dbd6-44d4-8fdf-c4b11a2c5073)



**Result:**Thus the Full adder and Full subtractor are studied and truth table is verified

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



