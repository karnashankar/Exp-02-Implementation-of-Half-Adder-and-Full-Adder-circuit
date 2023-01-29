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
##### Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.
### Program:
```
 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
 Developed by: Karna s 
 RegisterNumber:22008977
```
##### HALF ADDER:
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
##### FULL ADDER:
```
module full_adder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```

## Output:
### LOGIC SYMBOL & TRUTH TABLE: 
##### HALF ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317206-2fef6b9d-2d01-4dc2-8af7-96c0f3099b70.png)

##### FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317214-ef96138e-8baa-4f78-9e8d-0a1476847ec9.png)

### RTL REALIZATION:
##### HALF ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317250-f59c7c07-e024-40c2-83f6-2eda01072806.png)

##### FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317256-fb90d20b-2ccc-4aa6-9891-1471ceb88bcb.png)


### TIMING DIAGRAM

##### HALF ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317281-93b3d289-3b9a-448e-aa44-befb9726e2b2.png)


##### FULL ADDER:
![image](https://user-images.githubusercontent.com/121109150/215317297-b93ea9b7-4e64-4cb7-bfb4-27029d74f1c2.png)



### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
