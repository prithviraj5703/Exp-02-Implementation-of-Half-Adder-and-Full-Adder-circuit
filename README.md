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

 ![Screenshot 2023-04-13 120533](https://user-images.githubusercontent.com/121609342/231674369-094a0734-d10c-4dcf-b954-8e662f0fe8a7.png)


#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/121609342/231674533-c46acd9e-9fe4-476d-82e5-136a97defce6.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 

###Program:

```python
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: prithviraj
RegisterNumber:212222100038


HALF ADDER

module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule 

FULL ADDER

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule 
```
 
Logic symbol & Truthtable
RTL realization

### Output:

### HALF ADDER

### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/121609342/231674977-5adf488c-1388-4753-9512-7cfc868a3c59.png)

### RTL
![image](https://user-images.githubusercontent.com/121609342/231675013-160477f4-cb65-4eef-aa91-95bfd6a68db4.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/121609342/231675060-300f1038-14df-428b-bb5b-17150c820851.png)

### FULL ADDER

### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/121609342/231675144-d70b786b-690e-4ffd-9ad5-7a54097c5cc5.png)

### RTL
![image](https://user-images.githubusercontent.com/121609342/231675204-a0e69240-1e04-443e-80f0-04666b2df148.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/121609342/231675257-9c1fb508-68a8-4ef7-905e-aeb6fa6881f9.png)



### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
