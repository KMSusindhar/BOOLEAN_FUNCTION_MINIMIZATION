# BOOLEAN_FUNCTION_MINIMIZATION
Developed by: SUSINDHAR K M 
RegisterNumber: 212223040218

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
module de_exp_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (a & b & ~c) | (~a & b & d));
endmodule

```
```
module proj23(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&y)|(x&y));
endmodule
```


**TRUTH TABLE**'

F!

![image](https://github.com/user-attachments/assets/d00d62d7-40db-43ed-adf8-42c7e20ab0d7)

F2

![image](https://github.com/user-attachments/assets/cccd9b8e-5fb4-463c-b49a-f13ee4a56aba)



**RTL**

F1

![image](https://github.com/user-attachments/assets/d2fcaf88-33ac-4a57-bd11-dd43d297cb14)

F2

![image](https://github.com/user-attachments/assets/7b43d45b-e78c-4924-a768-6ea8f4907e34)


**Output:**
TIMING DIAGRAM

F1

![image](https://github.com/user-attachments/assets/38d80c37-42cd-4c98-b00b-8e7586d3c268)

F2

![image](https://github.com/user-attachments/assets/98173386-414d-4b4b-9f05-9ed9f51f79cc)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


