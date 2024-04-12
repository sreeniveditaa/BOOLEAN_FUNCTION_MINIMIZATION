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
Developed by: SREE NIVEDITAA SARAVANAN
RegisterNumber: 212223230213
```
```
module booleanfun(a,b,c,d,w,x,y,z,f1,f2);
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
and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule

```

**RTL realization**

![Screenshot 2024-04-12 131112](https://github.com/sreeniveditaa/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473268/ce16b4ad-c7d9-4776-9cde-f1c00779fc85)



**Timing Diagram**

![Screenshot 2024-04-12 131538](https://github.com/sreeniveditaa/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473268/0a3c6421-709a-481d-a81c-086634d9d85b)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

