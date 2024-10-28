# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
![WhatsApp Image 2024-10-28 at 2 25 28 PM](https://github.com/user-attachments/assets/c521b023-a49c-4693-a705-23169df809e2)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module ex_2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

module expl1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**
![ex_2](https://github.com/user-attachments/assets/2e1253b9-37a5-4e0d-be38-c726b079e7c6)
![WhatsApp Image 2024-10-28 at 2 34 29 PM](https://github.com/user-attachments/assets/8217da84-5bf2-40b6-8b8e-132e5c36d58d)


**Output:**
![WhatsApp Image 2024-10-28 at 2 44 49 PM](https://github.com/user-attachments/assets/bac24831-2ef2-4a2e-a156-b7e107a23907)
![WhatsApp Image 2024-10-28 at 2 45 18 PM](https://github.com/user-attachments/assets/0aa37f84-7fb1-4eb1-88b6-fdcd13fe3046)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

