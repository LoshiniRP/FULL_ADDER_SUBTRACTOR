# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**EQUIPMENTS REQUIRED:**

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

**TRUTH TABLE:**
![2](https://github.com/user-attachments/assets/abff08de-d5e2-4525-83c7-eb0e6885c9a6)


**PROCEDURE:**

Write the detailed procedure here

**PROGRAM:**
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
```
module exp4 (a,b,c,x,y,z,sum,dif,car,bor);
input a,b,c,x,y,z;
output sum,dif,car,bor;
assign sum = a^b^c;
assign car = a&b | a&c | b&c;
assign dif = x^y^z;
assign bor = ~x&z | ~x&y | y&z;
endmodule
```
Developed by: RegisterNumber: 25002119


**RTL:**
<img width="1920" height="1080" alt="Screenshot (79)" src="https://github.com/user-attachments/assets/3455ee59-3435-4ede-83f4-06b85a7a29bd" />



**TIMING WAVEFORM:**
<img width="1920" height="1080" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/29724f1f-ca3b-42c8-bdbf-c19c96ca6307" />


**RESULT:**

Thus, the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.
