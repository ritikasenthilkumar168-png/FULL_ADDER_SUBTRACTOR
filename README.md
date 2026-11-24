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
i) FULL ADDER
<img width="715" height="579" alt="image" src="https://github.com/user-attachments/assets/a63d0507-e6f7-4614-87bc-77bd8419a9bc" />

ii)FULL SUBTRACTOR
<img width="853" height="577" alt="image" src="https://github.com/user-attachments/assets/e9f76024-d1c3-4cc8-a763-b7c63735b12e" />


**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.*/
i)FULL ADDER
```
module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule
```
ii)FULL SUBTRACTOR
```
module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule
```
 Developed by: Ritika S
 Register Number: 212225220086

**RTL Schematic**
i) FULL ADDER
<img width="1042" height="457" alt="image" src="https://github.com/user-attachments/assets/d2765898-2ced-4b84-85aa-02c559ce5670" />

ii)FULL SUBTRACTOR
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/86271549-0d31-417a-a71c-0b58faf1a88d" />


**Output Timing Waveform**
i)FULL ADDER
<img width="1629" height="400" alt="image" src="https://github.com/user-attachments/assets/896b4af4-36cd-4dd3-938c-a671ba5b824e" />

ii)FULL SUBTRACTOR
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/edcc0011-a623-43cb-8dc1-62311a9f7dcc" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



