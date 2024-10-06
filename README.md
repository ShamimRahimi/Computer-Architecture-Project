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
