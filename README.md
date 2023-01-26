# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure
##### 1.Use module projname(input,output) to start the Verilog programmming.
##### 2.Assign inputs and outputs using the word input and output respectively.
##### 3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
##### 4.Use each output to represnt onre for differnce and the other for borrow.
##### 5.End the verilog program using keyword endmodule.
### Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
###### Developed by: Karna s 
###### RegisterNumber:22008977
*/


### Half subtractor :
###### module half_sub(output B,D, input x,y);
###### assign D=x^y;
###### assign B=~x&y;
###### endmodule

### Full subtractor :
###### module full_sub(output B,D, input x,y,z);
###### assign D=x^y^z;
###### assign B=(~x&(y^z))|(y&z);
###### endmodule


### Output:
### RTL
HALF ADDER:
![image](https://user-images.githubusercontent.com/121109150/214809593-0af26fb6-61b8-485e-b50b-146d4ef96e5b.png)
FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/214809694-940c45d9-11e9-4d32-82ee-0c2c427d6c10.png)

### TIMING DIAGRAM
HALF ADDER:
 
 
 ![image](https://user-images.githubusercontent.com/121109150/214809841-a774c2ca-469e-421a-aa44-0864ab8853f3.png)

FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/214809953-fa1d5d8f-b8ee-437d-a576-997571c40485.png)

### TRUTH TABLE 
##### HALF ADDER:
![image](https://user-images.githubusercontent.com/121109150/214810065-3e5b3ebc-1d46-4ff0-9639-6a302522d85a.png)

##### FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/214810125-82a7e27d-8ae9-4582-91fb-62906fe7c814.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
