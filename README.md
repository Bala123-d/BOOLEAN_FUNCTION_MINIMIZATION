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
```
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
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: D.BALA SUBRAMANYAM  RegisterNumber:24002856 */


**RTL realization**
![exp2-1](https://github.com/user-attachments/assets/5eb460aa-77cd-47c2-aa02-5fec105e144f)
![exp2-2](https://github.com/user-attachments/assets/98331d22-c9f9-441f-87e0-df3dd77d6154)

**Timing Diagram**
![exp2-3](https://github.com/user-attachments/assets/d1bc3219-cc72-4e8f-8923-5c01cc6dc50c)
![exp2-4](https://github.com/user-attachments/assets/af7f1251-03d6-4857-846d-8ef2cfae7e02)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

