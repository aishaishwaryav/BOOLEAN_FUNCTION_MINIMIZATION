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

Developed by:AISHWARYA V RegisterNumber:212223220003

program
module combinationalcircuit(A,B,C,D,F1);
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

RTL realization
![image](https://github.com/aishaishwaryav/BOOLEAN_FUNCTION_MINIMIZATION/assets/151565589/4b5078d6-21b4-4613-b63f-326e06965349)

Truth table
![image](https://github.com/aishaishwaryav/BOOLEAN_FUNCTION_MINIMIZATION/assets/151565589/6dfad3ec-2904-4ee6-96ab-bf73e924dbfc)

**Timing Diagram**
![image](https://github.com/aishaishwaryav/BOOLEAN_FUNCTION_MINIMIZATION/assets/151565589/aef1a2ba-b5af-4b61-8902-3c16b7ab9db0)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

