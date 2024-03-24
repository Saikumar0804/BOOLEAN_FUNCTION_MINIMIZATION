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

Developed by: Sai kumar.S
RegisterNumber:212222240087
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1 endmodule
```

**RTL realization**
![ED 2 1](https://github.com/Saikumar0804/BOOLEAN_FUNCTION_MINIMIZATION/assets/119280186/8e23a630-ec99-42ea-8b9f-078d97912d46)


**Output:**
![ED 2 2](https://github.com/Saikumar0804/BOOLEAN_FUNCTION_MINIMIZATION/assets/119280186/236e117e-87b8-48c3-9026-f0e1000cf845)

**RTL**
![ED 2 3](https://github.com/Saikumar0804/BOOLEAN_FUNCTION_MINIMIZATION/assets/119280186/07b435eb-fb74-4edb-9130-d1683ecc4eb1)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

