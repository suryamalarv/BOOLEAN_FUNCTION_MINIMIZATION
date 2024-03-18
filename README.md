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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. */
```
Developed by: surymalarv
RegisterNumber: 212223230224


 module program2(A,B,C,D,F1);
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
```



**RTL realization**

**Output:**

![image](https://github.com/suryamalarv/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742486/aaccd3bc-ae5e-4b35-b3be-1176c14134a9)





**Timing Diagram**

![image](https://github.com/suryamalarv/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742486/f06a8851-85e9-41ac-990c-c30976e9083a)


![image](https://github.com/suryamalarv/BOOLEAN_FUNCTION_MINIMIZATION/assets/145742486/53f361bd-1822-4141-b88f-de930b197d96)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

