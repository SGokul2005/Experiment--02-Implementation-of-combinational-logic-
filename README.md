# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
````
module kmap(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire A1,A2,A3,B1,B2,B3;
assign A1=(~a&(~b)&(~c)&(~d));
assign A2=(a&c&(~d));
assign A3=((~b)&c&(~d));
assign F1=A1|A2|A3;
assign B1=(x&(~y)&z);
assign B2=(~x&(~y)&z);
assign B3=(~w&x&y);
assign F2=B1|B2|B3;
endmodule
````
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
## RTL realization
![Screenshot 2024-01-01 191240](https://github.com/SGokul2005/Experiment--02-Implementation-of-combinational-logic-/assets/147121825/04cb4926-95c4-4c88-90d9-f4e7395e3a75)
![Screenshot 2024-01-01 191422](https://github.com/SGokul2005/Experiment--02-Implementation-of-combinational-logic-/assets/147121825/37259fed-b527-4221-8d50-bb86710e0d7c)
![Screenshot 2023-12-31 131453](https://github.com/SGokul2005/Experiment--02-Implementation-of-combinational-logic-/assets/147121825/9444e694-2f25-47d8-8161-603b363dab07)


## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
