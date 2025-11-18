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
![WhatsApp Image 2025-11-18 at 11 05 56_2567dbd6](https://github.com/user-attachments/assets/e50f777a-7e1b-4ceb-a432-dccb4fc1cc58)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Arjun.R.S RegisterNumber: 25017547*/
```
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

**RTL realization**
<img width="1920" height="1080" alt="Screenshot 2025-11-12 213606" src="https://github.com/user-attachments/assets/07ba0430-02a7-4659-91f6-80498194f847" />



**RTL**

<img width="1920" height="1080" alt="Screenshot 2025-11-12 215253" src="https://github.com/user-attachments/assets/52dcafe1-d2c5-48ae-9eba-2467b44899a0" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

