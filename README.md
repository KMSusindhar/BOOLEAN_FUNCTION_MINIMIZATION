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
module boolean_minimization(a,b,c,d,w,x,y,z,f1,f2);
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

Developed by: SUSINDHAR K M 
RegisterNumber: 212223040218


**TRUTH TABLE**'
![image](https://github.com/user-attachments/assets/a851337e-1ae3-4c03-b3b6-5144049fc6b5)
![image](https://github.com/user-attachments/assets/d419c4e8-393d-434b-9c7c-c864aaefa30e)

**RTL**
![image](https://github.com/user-attachments/assets/6849ae59-2540-43cf-bc29-f6645362ba3b)
**Output:**
![image](https://github.com/user-attachments/assets/faa0165c-8936-4563-88e4-ff3ab380a2fd)

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


