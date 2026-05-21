# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SAHANA G
RegisterNumber: 212225040354
```
module booleanexpression (
    input A, B, C, D,
    output F
);

wire nB, nD, term1, term2, term3;

// NOT gates
not (nB, B);
not (nD, D);

// AND terms
and (term1, nB, nD); // B'D'
and (term2, A, C);   // AC
and (term3, B, D);   // BD

// OR the terms
or (F, term1, term2, term3);

endmodule
```

**RTL realization**

**Output:**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9e91c339-1868-4a6a-86e0-79a180adc3a0" />

**RTL**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/98ab0285-e7e2-4265-8948-93968d0ab494" />

**Timing Diagram**

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

