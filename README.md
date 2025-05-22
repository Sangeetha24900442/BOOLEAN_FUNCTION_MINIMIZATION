# BOOLEAN FUNCTION MINIMIZATION

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

Developed by: Sangeetha.S
RegisterNumber:212224040287

```
module ex2(A,B,C,D,F1,W,X,Y,Z,F2);
input A,B,C,D,W,X,Y,Z;
output F1,F2;
wire x1,x2,x3,x4,x5,x6;
assign x1=(~B)&(~D);
assign x2=A&B&(~C);
assign x3=(~A)&(B)&(D);
assign x4=(~Y)&(Z);
assign x5=(X)&(Y);
assign x6=(W)&(Y);
assign F1=x1|x2|x3;
assign F2=x4|x5|x6;
endmodule
```


**RTL realization**

![Screenshot 2025-04-24 105501](https://github.com/user-attachments/assets/e405fb9b-7029-43f5-82ce-e7cdd742d40a)



**Output:**

![image](https://github.com/user-attachments/assets/7cb2dc09-9e45-487a-917d-7783a4e6473a)


**Timing Diagram**

![Screenshot 2025-04-24 105909](https://github.com/user-attachments/assets/6e225964-4405-4e80-a431-a026245cf5d5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

