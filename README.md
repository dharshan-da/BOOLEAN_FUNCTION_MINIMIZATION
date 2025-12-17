# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of reducing a Boolean expression to its simplest form.
It removes unnecessary terms and variables to create an efficient logic circuit.
The minimized form uses fewer gates, reducing cost and power.
Methods include algebraic simplification, K-Maps, and the Quine–McCluskey method.

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


i)
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule


ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

Developed by/ RegisterNumber:DHARSHANSHRI DA/25017586


**RTL realization**
<img width="1064" height="544" alt="image" src="https://github.com/user-attachments/assets/25207c0e-450d-42f0-8042-77955ad32893" />

<img width="1026" height="539" alt="image" src="https://github.com/user-attachments/assets/42031d01-a7b8-48a7-81d6-d2a0d8156d0b" />


**Output:**
<img width="1043" height="525" alt="image" src="https://github.com/user-attachments/assets/82a2a862-1b90-428f-8734-e7daa5eaeb63" />

<img width="1034" height="494" alt="image" src="https://github.com/user-attachments/assets/b9e1c246-6005-42da-b75d-cf6f2a3021f1" />

*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

