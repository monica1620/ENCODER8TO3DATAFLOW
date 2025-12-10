### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

1. Open Quartus Prime and create a new project.
2. Create a Verilog HDL file and enter the program for the 8-to-3 encoder.
3. Save the file and compile the program.
4. Open the RTL Viewer to view the logic diagram.
5. Create a new Vector Waveform File (.vwf) for simulation.
6. Add all the input and output signals to the waveform.
7. Apply the input values according to the truth table.
8. Run the simulation and observe the output waveforms.
9. Compare the simulated outputs with the truth table.

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 


//*8 Developed by: Monica R
//* Register Number: 25010138

module experi5(D, A);
input [7:0] D;     
output [2:0] A;     
assign A[0] = D[1] | D[3] | D[5] | D[7];
assign A[1] = D[2] | D[3] | D[6] | D[7];
assign A[2] = D[4] | D[5] | D[6] | D[7];
endmodule


**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/89184457-c293-4c25-92a3-1ffb0a126c1b" />


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/18b96c3f-b12b-48a9-a6b1-61b872be40a0" />


**RESULTS**
The Encoder 8-to-3 was successfully implemented using Dataflow Modelling in Verilog.
The simulated outputs match exactly with the truth table, verifying correct functionality.



