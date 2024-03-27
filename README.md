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
module booleanfun(F1,F2,A,B,C,D);
output F1,F2;
input A,B,C,D;
assign F1=(~A&~B&~C&~D)|(A&~C&~D)|(~B&C&~D)|(~A&B&C&D)|(B&~C&D);
assign F2=(B&~C&D)|(~B&~C&D)|(~A&B&C)|(A&~B&C)|(A&B&C);
endmodule

```

**RTL realization**

![image](https://github.com/sreeniveditaa/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473268/686f655f-d8d2-4015-a331-680a6e54b0df)

**Output:**


**Timing Diagram**

![image](https://github.com/sreeniveditaa/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473268/bb008a70-fec6-43ef-9953-ab634041cc83)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

