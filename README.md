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

Developed by:R.DEEPIKA    RegisterNumber:24900220
```
module bbb(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign x6=(x)&(~y)&(z);
assign x7=(~x)&(~y)&(z);
assign x8=(~w)&(x)&(y);
assign x9=(w)&(~x)&(y);
assign x10=(w)&(x)&(y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```

**RTL realization**![image](https://github.com/user-attachments/assets/9a16fddb-a573-4e81-b768-32e0c5e6f9ed)


**Output:**![image](https://github.com/user-attachments/assets/0335c9bd-3c20-449d-af98-dd69fc00ad4a)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

