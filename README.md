# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
1.Create a NewProject:

2.Open Quartus and create a new project by selecting "File" > "New Project Wizard."

3.Followthewizard'sinstructionstosetupyourproject,includingspecifyingtheprojectname, location, and target device(FPGA).
  >Create a New DesignFile:
       *Oncetheprojectiscreated,right-clickontheprojectnameintheProjectNavigatorandselect "Add NewFile."
       *Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.
4.Write the Combinational LogicCode:
  >Open the newly created Verilog or VHDL file and write the code for your combinational logic.
5.Compile theProject:
  >To compile the project, click on "Processing" > "Start Compilation" in the menu.
  >Quartuswillanalyzeyourcode,synthesizeitintoanetlist,andperformoptimizationsbasedon your target FPGAdevice.
6.Analyze and FixErrors:
  >If there are any errors or warnings during the compilation process,Quartus will display them in the Messages window.
  >Reviewandfixanyissuesinyourcodeifnecessary. View the RTLdiagram.
7.Verification:
  >Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
  >OnceWaveformiscreatedRightClickontheInput/OutputPanel>"InsertNodeorBus">Click onNodeFinder>ClickOn"List">SelectAll.
  >Give the Input Combinations according to the Truth Table amd then simulate the Output Waveform.

Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Prasanna A
RegisterNumber:  23005675

## Program:

Half Subractor:

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/14867b75-5c7a-4a4c-95f4-7031d971a93b)

Full Subractor:

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/4b90f091-9926-4860-b01b-2271ee0afe70)

## Truthtable

HALF SUBRACTOR

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/d9fc9a59-8fb2-4e97-bb4d-0612b4ef6da5)

FULL SUBRACTOR

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/eb36c795-96bb-4f82-9a68-cad2c529ee31)

##RTL realization

HALF SUBRACTOR

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/87389006-1f5f-49b1-9063-49344a1f87df)

FULL SUBRACTOR

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/28ebbdcf-3532-44a1-bf3d-cd2b734457ee)

##Timing diagram

Half subractor

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/89f824fa-ebac-4bca-8cea-133f8aa5f2f4)

Full subractor

![image](https://github.com/prasanna-765/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150009505/ec76b16b-58b3-495d-b32f-006704ffbb8a)


## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
