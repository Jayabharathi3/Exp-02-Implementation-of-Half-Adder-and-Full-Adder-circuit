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
/*
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: JAYABHARATHI.S
RegisterNumber: 212222100013
/*

HALF ADDER:

module halfadder(a,b,c,s);
input a,b;
output s,c;
xor(s,a,b);
and(c,a,b);
endmodule

FULL ADDER:

module fulladder(x,y,z,s,c,x1,x2,x3,x4);
input x,y,z;
output s,c,x1,x2,x3,x4;
xor(x1,x,y);
xor(s,x1,z);
and(x3,x,y);
and(x4,x1,z);
or(c,x3,z);
endmodule 
```

### Output:

### TIMING DIAGRAM

HALF ADDER
![half adder time](https://user-images.githubusercontent.com/120367796/232683223-f9743a16-702c-4914-981e-10a3cd6fb7b7.png)

FULL ADDER
![image](https://user-images.githubusercontent.com/120367796/232683146-987f2322-014e-422a-a906-ab5c0fffac93.png)


### RTL

HALF ADDER
![image](https://user-images.githubusercontent.com/120367796/232683957-510252ee-e3a4-48f8-b26a-3eeba488c2b5.png)

FULL ADDER
![full adder rtl](https://user-images.githubusercontent.com/120367796/232684002-09fc37c4-9bb3-4289-b179-0c2fc6ad81f0.png)


## TRUTH TABLE

HALF ADDER

![image](https://user-images.githubusercontent.com/120367796/232685416-a5699dea-43d3-4646-8470-cb23fd7e298c.png)

FULL ADDER

![image](https://user-images.githubusercontent.com/120367796/232685444-c72487f6-55a7-47ff-a594-3c5d861bb208.png)


## LOGIC SYMBOL

HALF ADDER

![ha logic](https://user-images.githubusercontent.com/120367796/232685258-6de83d55-4bf3-4ca5-bf2a-9bda62f025ad.png)

FULL ADDER

![image](https://user-images.githubusercontent.com/120367796/232685330-4ec237b6-ae9e-4f89-82b4-26ec467b45a9.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.

