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

Truth Table 1:
![image](https://github.com/user-attachments/assets/cd7be267-7c4d-4a2b-9221-718f22965db2)

Truth Table 2:

![image](https://github.com/user-attachments/assets/1706abec-b946-4185-9b07-827ba0626e73)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SRUTHI A

RegisterNumber: 212224240162*/

module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


**RTL realization**

**Output:**

![image](https://github.com/user-attachments/assets/6c49e64e-bc8a-42fa-aaf1-f0dc6935dde7)

![image](https://github.com/user-attachments/assets/1dfb74a3-12ed-498c-b48b-38237d98224d)

**RTL**

![image](https://github.com/user-attachments/assets/4e3f6c5e-1afa-4319-a8a2-076380c989df)

![image](https://github.com/user-attachments/assets/4795cf0f-f711-4167-824d-c98d0e12ee39)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

