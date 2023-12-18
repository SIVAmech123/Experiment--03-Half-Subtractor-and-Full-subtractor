## Name:R.Sivakumar
## Ref :23013501
# #Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime

## Theory:
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor:

## Half Subtractor:
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure:
## A.Half adder
1. A half subtractor is a combinational circuit that performs the subtraction of two single-bit numbers and produces two outputs: the difference and the borrow.

2. Let's consider two single-bit inputs A and B.

3. Difference (Diff): This output represents the result of the subtraction A - B and is obtained by performing an XOR operation on inputs A and B.

4. Borrow (Borrow): This output indicates whether a borrow is required for the subtraction and is obtained by performing an AND operation between the complement of A and B.
## B.Full adder:
1. A full subtractor is a combinational circuit that subtracts three single-bit inputs: A, B, and a Borrow-In (Bin), and produces two outputs: the difference and a Borrow-Out (Bout) to the next subtractor in a sequence.

2. Difference (Diff): This output represents the result of the subtraction A - B - Bin.

3. Borrow-Out (Bout): This output indicates whether a borrow is required for the subtraction and will be used in further subtractors.

4. A full subtractor is typically constructed using two half subtractors. The Borrow- Out of the first half subtractor is used as an input Borrow-In for the second half subtractor. The outputs of the half subtractors are combined to generate the final Difference and

## Program:
## HALFSUBTRACTOR:

<img width="203" alt="Screenshot 2023-12-18 210230" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/a72e7046-cd00-465f-bbf3-14bd4aabe331">

## FULLSUBTRACTOR:

<img width="209" alt="Screenshot 2023-12-18 210247" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/7b557b67-cc38-478a-888d-a807ff797841">


## Output:

##  RTL realization:
<img width="273" alt="Screenshot 2023-12-18 132854" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/d97b3505-2587-476f-9b89-b4c53ea65b29">
<img width="423" alt="Screenshot 2023-12-18 132902" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/53bca56d-3089-4ea3-8d7f-b6d087d0d0db">

## Truth table:
<img width="365" alt="Screenshot 2023-12-18 132916" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/49397127-580b-4e4a-9808-69a756a6c7f7">
<img width="378" alt="Screenshot 2023-12-18 132930" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/fc2adb80-7133-4276-8b84-e80a1add518e">


## Timing diagram :

<img width="601" alt="Screenshot 2023-12-18 132945" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/3875e799-cc86-4576-ba74-3df965372bf6">
<img width="604" alt="Screenshot 2023-12-18 132956" src="https://github.com/SIVAmech123/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/151629067/775cea5b-e3ba-4099-878e-0db8bfd01969">

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
