NAME:K.Abhineswar Reddy<br>
REFERENCE NUMBER:212223040084
# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/e0f7e18e-7dad-46cd-ad7f-18420202df3f)

 
#### Figure -01 HALF ADDER 
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/8797e5e4-4ce2-40ef-8d2a-505097e13576)


#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows. 

Program:
# Half Adder:


module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule



# Full Adder


module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule



### TRUTH TABLE 
Half Adder Circuit:
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/d020a304-f4c2-4a4b-9114-551f43a9bb0d)


Full Adder Circuit:-
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/1031e70b-e4cb-4d91-8182-1bfbc53041e1)


### RTL
Half Adder Circuit:
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/145a3f18-34c1-4cd7-8fb6-45b8fa07ea5e)


Full Adder Circuit:-
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/3d09728b-9123-422e-bf7b-5e51284701f0)


### Output:
Half Adder Circuit:-
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/78f6351b-62ee-40d5-96d7-854cdd02a44e)


Full Adder Circuit:-
![image](https://github.com/23012312/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150009714/77ff4212-0fd2-4bd4-bb46-be6e5de97c1d)


### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.






































