# ALU-Based Digital Calculator Using SystemVerilog

## About the Project
A digital calculator designed using an Arithmetic Logic Unit (ALU). The system accepts two 8-bit operands and selects the required operation through a 4-bit control opcode. The design is implemented using SystemVerilog combinational logic.

## Functional Capabilities

The calculator supports the following operations:

### Arithmetic Operations
- Addition
- Subtraction
- Multiplication
- Division

### Logical Operations
- Bitwise AND
- Bitwise OR
- Bitwise XOR
- Bitwise NOT

## Opcode Selection

| Control Opcode | Selected Function |
|---|---|
| 0000 | ADD |
| 0001 | SUB |
| 0010 | MUL |
| 0011 | DIV |
| 0100 | AND |
| 0101 | OR |
| 0110 | XOR |
| 0111 | NOT |

## Design Architecture

The design consists of two main modules:

**1. Digital Calculator Module**
- Receives operands A and B.
- Decodes the opcode.
- Executes the selected arithmetic or logical operation.
- Produces a 16-bit result.
- Generates operation status indicators.
- Includes internal carry, borrow, zero and division-by-zero flags.

**2. Verification Module**
- Applies different input combinations.
- Tests all eight supported operations.
- Generates simulation waveforms in VCD format.

## Technical Specifications

| Parameter | Value |
|---|---|
| HDL | SystemVerilog |
| Operand size | 8 bits |
| Control input | 4 bits |
| Result size | 16 bits |
| Design methodology | Combinational |
| Simulation platform | EDA Playground |

## Simulation

The design is verified using a SystemVerilog testbench. Different operand combinations are applied to check the functionality of each operation. The generated VCD waveform can be used to inspect the input and output signal transitions.

## Applications
- Understanding ALU operation and opcode decoding
- Learning digital system design
- Practicing SystemVerilog coding
- Studying combinational arithmetic and logic circuits

## Author
Dharshini Priya
