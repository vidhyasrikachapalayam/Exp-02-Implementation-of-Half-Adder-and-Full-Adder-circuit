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

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: vidhyasri.k
RegisterNumber:  212222230170
```
half adder
module exp3 (a,b,sum,carry);

input a,b;

output sum,carry;

assign sum = (a^b);

assign carry = (a&b);

endmodule

Full adder
module exp3f (a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = (a^b^c);

assign carry = ((a&b)|(a^b)&c);

endmodule
### Output:
### RTL
## Halfadder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/2b019c39-15da-401d-8a91-c1d103c486a2)
## Fulladder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/6a4bfa73-5fcb-48d9-bde5-1e7d347d648b)


### TIMING DIAGRAM
## Halfadder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/9bdd8ad7-5fd3-457e-8481-5fbafdbbbd8a)
## Fulladder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/41f3d82c-08c1-4c18-bb32-fe8786535c85)



### TRUTH TABLE 
##Halfadder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/76d22e8d-9c16-483f-a86d-97010d36007a)
##Fulladder
![image](https://github.com/vidhyasrikachapalayam/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119477817/a5313912-38be-4892-a629-28e6c35d2b93)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
