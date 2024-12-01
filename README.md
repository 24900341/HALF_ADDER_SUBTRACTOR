**EXP3: HALF ADDER AND SUBTRACTOR**

NAME: A.MOHAMED NIZAMUDDIN

REF NO: 24900341


**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

1)HALF ADDER

![image](https://github.com/user-attachments/assets/2e8b080b-5d7c-4d2b-a2b6-2a2ea9db8c8e)

2)HALF SUBRACTOR

![image](https://github.com/user-attachments/assets/8c762da0-936e-4762-93ca-b0bd9fe203e3)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

i)HALF ADDER

module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

ii)HALF SUBRACTOR


module halfsubractor(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule


**RTL Schematic**

1)HALF ADDER

![screen shot of half adder](https://github.com/user-attachments/assets/ae607d99-b8b8-4135-bb16-164b816109a6)


2)HALF SUBRACTOR

![screenshot of half subractor](https://github.com/user-attachments/assets/92a0eff7-49b1-4e8b-a65c-aaaaa3885c40)



**Output/TIMING Waveform**

1)HALF ADDER

![wave form of half adder](https://github.com/user-attachments/assets/f2911ac9-6f27-45ee-bac8-c7fc414ff11a)


2)HALF SUBRACTOR

![wave form of half subractor](https://github.com/user-attachments/assets/38001370-cb52-43cf-a300-486240dac537)

**RESULT:**

Thus the  half adder and half subtractor circuit  is designed and verified its truth table in Quartus using Verilog programming.

