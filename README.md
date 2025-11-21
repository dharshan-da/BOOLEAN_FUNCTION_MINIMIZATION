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

module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(w&y)|(x&y));
endmodule

Developed by/ RegisterNumber:DHARSHANSHRI DA/25017586


**RTL realization**
<img width="1920" height="1080" alt="Screenshot 2025-11-17 135614" src="https://github.com/user-attachments/assets/1c8b24ac-25a4-4d27-80bc-18e50bbf87eb" />


**Output:**
![WhatsApp Image 2025-11-17 at 13 59 33_99697faf](https://github.com/user-attachments/assets/eef20f09-cc13-453b-807f-732018ab7b10)
*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

