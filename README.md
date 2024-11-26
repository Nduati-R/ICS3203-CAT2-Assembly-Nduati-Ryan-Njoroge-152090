# ICS3203-CAT2-Assembly-Nduati-Ryan-Njoroge-152090

## Overview
This repository contains four assembly programs developed as part of the ICS3203 CAT 2 practical assignment. Each program demonstrates specific assembly language techniques such as control flow, array manipulation, modular programming, and port-based simulations.

## Repository Structure
ICS3203-CAT2-Assembly-<Nduati Ryan Njoroge-152090>
│
├── README.md
├── task1.asm  # Control Flow and Conditional Logic
├── task2.asm  # Array Manipulation with Looping and Reversal
├── task3.asm  # Modular Program with Subroutines for Factorial Calculation
└── task4.asm  # Data Monitoring and Control Using Port-Based Simulation


## Task Descriptions

### 1. **Control Flow and Conditional Logic** (`task1.asm`)
This program prompts the user to input a number and classifies it as:
- **POSITIVE**
- **NEGATIVE**
- **ZERO**

#### Key Features:
- Uses **conditional jumps** (`je`, `jl`) to classify the number.
- Includes an **unconditional jump** (`jmp`) for program flow control.

#### Insights:
- Implementing proper branching ensured clarity and ease of debugging.
- Managing conditional and unconditional jumps helped organize the logic.

---

### 2. **Array Manipulation with Looping and Reversal** (`task2.asm`)
This program accepts an array of integers and reverses the array in place without using additional memory.

#### Key Features:
- Employs a **loop** to swap array elements directly.
- Uses **pointers** to manage array indices.

#### Insights:
- Managing in-place reversal without extra memory required careful pointer logic.
- Ensuring the loop exits correctly when pointers meet was a critical aspect.

---

### 3. **Modular Program with Subroutines for Factorial Calculation** (`task3.asm`)
This program calculates the factorial of an input number using a recursive subroutine.

#### Key Features:
- Demonstrates **modular programming** using a subroutine.
- Uses the **stack** to preserve and restore registers during recursion.
- Final result is stored in a general-purpose register.

#### Insights:
- Stack management was crucial for maintaining register integrity during recursion.
- Recursive implementation highlighted the importance of efficient stack operations.

---

### 4. **Data Monitoring and Control Using Port-Based Simulation** (`task4.asm`)
This program simulates sensor-based control actions:
- **Motor control**: Starts/stops the motor based on sensor input.
- **Alarm trigger**: Activates an alarm when the sensor value exceeds a threshold.

#### Key Features:
- Simulates **sensor values** and actions using memory locations.
- Demonstrates logic to handle multiple actions based on conditions.

#### Insights:
- Simulating hardware control in assembly required creative use of memory.
- Defining thresholds and managing program flow ensured correct behavior.

---

## Compilation and Execution

### **Prerequisites**
- An assembler such as **NASM** or **MASM**.
- A 64-bit or 32-bit environment compatible with the chosen assembler.

### **Compilation**
To compile the programs, use the following commands (for NASM as an example):
```bash
nasm -f elf64 task1.asm -o task1.o
ld task1.o -o task1
./task1



