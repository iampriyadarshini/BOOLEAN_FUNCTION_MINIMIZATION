 ### NAME : PRIYADARSHINI K
 ### REGISTER NO: 24900922
 ### EXPERIMENT 2: BOOLEAN FUNCTION MINIMIZATION 

# AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

# EXPERIMENT REQUIRED :

Hardware – PCs, Cyclone II , USB flasher

 SOFTWARE – QUARTUS PRIME :

## THEORY
Implementing Boolean functions in Verilog HDL (Hardware Description Language) involves translating the simplified Boolean expressions into Verilog code to describe the behavior of digital circuits. The basic building blocks in Verilog is module. The module represent a combinational circuit. Use logical operators (&, |, ~, ^) to implement Boolean functions directly. Use built-in gate primitives for basic functions. Use University program VWF to verify the functionality of your Verilog modules. Create waveform and check outputs against expected results.



## PROCEDURE

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## PROGRAM 
module EX2 (a,b,c,d,w,x,y,z,f1,f2); </br>
input a,b,c,d,w,x,y,z;

output f1,f2;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

assign x1=(~a)&(~b)&(~c)&(~d);

assign x2=(~a)&(~c)&(~d);

assign x3=(~b)&(c)&(~d);

assign x4=(~a)&(b)&(c)&(~d);

assign x5=(b)&(~c)&(d);

assign x6=(x)&(~y)&(z);

assign x7=(~x)&(~y)&(z);

assign x8=(~w)&(x)&(y);

assign x9=(w)&(~x)&(y);

assign x10=(w)&(x)&(y);

assign f1=x1|x2|x3|x4|x5;

assign f2=x6|x7|x8|x9|x10;

endmodule

## TRUTH TABLE
![TRUTHTABLE](https://github.com/user-attachments/assets/db359a55-25d0-40bb-a58f-a1905111e01f)


## RTL OUTPUT
![RTL OUTPUT](https://github.com/user-attachments/assets/bed75bdd-f01c-405b-9cc6-e846cee4709b)


## OUTPUT WAVEFORM
![OUTPUT WAVEFORM](https://github.com/user-attachments/assets/6920efb1-51d8-44ab-81f7-9354d6a47d3b)




## RESULT:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

