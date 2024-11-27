# HALF_ADDER_SUBTRACTOR

**EXP 3: HALF ADDER AND SUBRACTOR**

NAME: A. MOHAMED NIZAMUDDIN

REG NO: 24900341

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

i)HALF ADDER TRUTH TABLE:

![image](https://github.com/user-attachments/assets/80eb936b-32d2-4bb5-9104-88483f371dcf)

ii)HALF SUBRACTOR TRUTH TABLE:

![image](https://github.com/user-attachments/assets/6bae51bf-5a46-49b7-adfd-30e4091c9d59)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

i)HALF ADDER:-
module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

ii)HALF SUBRACTOR:-

module halfsubractor(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule

**RTL Schematic**

i)HALF ADDER:-

![screen shot of half adder](https://github.com/user-attachments/assets/98be02f8-aea5-4695-86cb-4f3790372389)


ii)HALF SUBRACTOR:-

![screenshot of half subractor](https://github.com/user-attachments/assets/b750a9a5-3450-41dc-bbe9-a5ed8586e78c)


**Output/TIMING Waveform**

i)HALF ADDER:-

![wave form of half adder](https://github.com/user-attachments/assets/89cc1557-a485-4e92-8a00-a99518e51339)


ii)HALF SUBRACTOR:-

![wave form of half subractor](https://github.com/user-attachments/assets/3ad194aa-eb62-4043-80b2-7a37a1fc1cd5)



**Result:**
Thus a half adder and half subtractor circuit is designed and its truth table in Quartus using Verilog programming  is verified.

