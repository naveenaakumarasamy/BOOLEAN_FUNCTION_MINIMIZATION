# EX NO:2 BOOLEAN_FUNCTION_MINIMIZATION

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

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:NAveenaa A K

RegisterNumber:212222230094
```
module exp22(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule

```
**RTL realization**

![image](https://github.com/Hemasonica774/BOOLEAN_FUNCTION_MINIMIZATION/assets/118361409/ed911319-3d25-4ad8-be85-1145b1fd0f8f)

**Truth table**

![image](https://github.com/Hemasonica774/BOOLEAN_FUNCTION_MINIMIZATION/assets/118361409/af782e45-7db6-4eb4-8db6-d8f3b73b310c)

**Timing Diagram**

![image](https://github.com/Hemasonica774/BOOLEAN_FUNCTION_MINIMIZATION/assets/118361409/22cb916b-719e-407f-a1af-9768d661857b)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

