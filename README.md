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
```python
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SAELVA KUMAR A
RegisterNumber: 22009007 
~~~
Half Adder Program:

module HalfAdder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

Full Adder Program:

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=((a^b)^c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule
*/
```
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
### Half Adder:
![image](https://user-images.githubusercontent.com/120643262/231696605-4c11e7d3-2195-43aa-8074-7484fa297509.png)
### Full Adder:
![image](https://user-images.githubusercontent.com/120643262/231697124-85c73d5a-c506-4898-8958-05ae84aad9cc.png)

### TIMING DIAGRAM
### HALF ADDER:
![image](https://user-images.githubusercontent.com/120643262/231697219-2f4784a6-3d47-4a32-91c4-75af7ad73c06.png)
### FULL ADDER:
![image](https://user-images.githubusercontent.com/120643262/231697580-973b8b06-eaa5-4fff-817d-e37d87154d9a.png)



### TRUTH TABLE 
### HALF ADDER:
![image](https://user-images.githubusercontent.com/120643262/231697816-135c0bad-116c-4faa-93a8-6da1dfedd4ff.png)

### FULL ADDER:
![image](https://user-images.githubusercontent.com/120643262/231698159-a406c659-7fc1-43ae-9a31-64bb4e18ab3c.png)


### Result:
