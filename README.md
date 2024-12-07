# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: KESHAVARTHINI B          RegisterNumber:*/ 24900033

module boolean_mini(a,b,c,d,w,x,y,z,f1,f2);

input a, b, c, d,w,x,y,z;  

output f1, f2;     

assign f1 = (~a & ~b & ~c & ~d) | (a&~c&~d) | (~b&c&~d) | (~a&b&c&d) | (b&~c&d);

assign f2 = (x&~y&z) | (~x&~y&z) | (~w&x&y) | (w&~x&y) | (w&x&y);

endmodule


**RTL realization**

![Screenshot (39)](https://github.com/user-attachments/assets/330b7fad-e8bb-474a-bfc9-ffb3adbc7868)


**Output:**

**RTL**

![Screenshot (38)](https://github.com/user-attachments/assets/c41a176a-3ffd-43b5-8100-22045dbc169d)


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

