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


## Program:
**Developed by: Naveenaa A K**  
**RegisterNumber: 212222230094** 

```
module BMf1f2(a,b,c,d,w,x,y,z,f1,f2);
  input a,b,c,d,w,x,y,z;
  output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
  not(adash,a);
  not(bdash,b);
  not(cdash,c);
  not(ddash,d);
  and(p,bdash,ddash);
  and(q,adash,b,d);
  and(r,a,b,cdash);
  or(f1,p,q,r);
//type code for f2 as like f1
 not(ydash,y);
 and(s,x,y);
 and(t,ydash,z);
 and(u,w,y);
 or(f2,s,t,u);
endmodule
```

## RTL realization output
![image](https://github.com/subha-shinibalasubramanian/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154478/4a409975-f89a-44a5-8985-11b5c0bc4503)


## Timing Diagram
![image](https://github.com/subha-shinibalasubramanian/BOOLEAN_FUNCTION_MINIMIZATION/assets/164154478/a999da2b-37a5-4382-b852-f12fe444671b)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

