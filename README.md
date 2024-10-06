# Computer-Architecture-Project

# 4-Bit Serial Adder-Based Multiplier

This project implements a 4-bit binary multiplier by adding the number \(A\) repeatedly, based on the value of \(B\). The multiplication is done by controlling how many times \(A\) is added to itself, simulating the multiplication process.

## Overview

- **Method**: The circuit performs multiplication by adding \(A\) to itself \(B\) times.
- **Structure**: 
  - The first row consists of 7 adders that sum \(A\) with itself.
  - The second row has 4 adders that sum the outputs of the first row.
  - The third row has 2 adders, summing the outputs of the second row.
  - The last row has 1 adder that sums the outputs of the third row.
  
- **Multiplexers**: 2-to-1 multiplexers are used to control when \(A\) is added or when the value is set to zero, depending on the binary value of \(B\).

## Operation

- The circuit takes two 4-bit inputs, \(A\) and \(B\).
- It multiplies \(A\) by adding it \(B\) times, controlled by multiplexers.
- A combination circuit generates control signals based on the value of \(B\) to ensure the correct number of additions.

## Files

- **Circuit Design Files**: Proteus simulation files for the multiplier circuit.
- **Images**: Pictures of the circuit setup.

# 4-Bit Multiplier/Divider Circuit

This project implements a 4-bit hardware multiplier and divider. The circuit can switch between multiplication and division modes based on the control bit `M`.

## Overview

- **Multiplier/Divider Control**: The bit `M` determines the operation mode:
  - `M = 0`: The circuit performs multiplication.
  - `M = 1`: The circuit performs division.
  
- **Components**:
  - **4-bit ALU**: Performs arithmetic operations on the inputs.
  - **Multiplicand/Divisor**: 4-bit input for the operation.
  - **Product/Remainder**: 8-bit output of the operation.
  - **Shift and Write Units**: Used to shift and write intermediate results during the multiplication or division process.
  - **Control Unit**: Manages the flow and determines when to shift, write, or stop based on the operation.
  
## Operation Modes

1. **Multiplication**:
    - The circuit multiplies two 4-bit inputs and stores the result in a 8-bit product register.
    - Shifting is applied to handle binary multiplication.
   
2. **Division**:
    - The circuit divides two 4-bit inputs, returning a 4-bit quotient and a 4-bit remainder.
    - Shifting is used to align bits during the division process.

## Circuit Design

The design includes:
- **Multiplexers** to switch between multiplication and division.
- **Registers** to store intermediate results.
- **Control Logic** that directs operations based on the value of `M`.

## Files

- **Design Files**: Proteus simulation files for the multiplier/divider circuit.
- **Images**: Pictures of the circuit setup, including a snapshot of the control and ALU logic.

