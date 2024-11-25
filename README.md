# ICS3203-CAT2-Assembly-Beldi_Muhindo_Kamuha_147886

Overview

This repository contains four assembly language programs designed to demonstrate fundamental concepts such as control flow, modular programming, data monitoring, and array manipulation. Each program is built with efficiency and clarity in mind, using assembly techniques to solve specific tasks.

Programs

	1.	Number Classification
	•	Purpose: Classify a user-input number as POSITIVE, NEGATIVE, or ZERO.
	•	Highlights: Utilizes conditional and unconditional jumps to determine the classification and display results.
	2.	Array Reversal
	•	Purpose: Accepts an array of five integers, reverses it in place, and outputs the reversed array.
	•	Highlights: Implements in-place reversal using loop-based two-pointer logic without requiring extra memory.
	3.	Factorial Calculation
	•	Purpose: Computes the factorial of a user-input number (0–12) using modular programming principles.
	•	Highlights: Demonstrates register preservation with stack usage and modularity through a dedicated factorial subroutine.
	4.	Sensor Control Simulation
	•	Purpose: Simulates sensor-based control logic for a motor and alarm based on water-level thresholds.
	•	Highlights: Implements control thresholds (LOW, MODERATE, and HIGH) and updates memory locations to simulate hardware behavior.
 Compilation and Execution

Requirements

	•	A Linux-based operating system or an emulator capable of handling syscalls.
	•	NASM (Netwide Assembler) for assembling the code.
	•	ld (GNU Linker) for linking the object files.

Steps to Compile and Run

1.	Task 1 Number Classification:
nasm -f elf64 task_1.asm -o task_1.o
ld task_1.o -o task_1
./task_1

2.	Task 2 Array Reversal:
nasm -f elf64 task_2.asm -o task_2.o
ld task_2.o -o task_2
./task_2

3.	Task 3 Factorial Calculation:
nasm -f elf64 task_3.asm -o task_3.o
ld task_3.o -o task_3
./task_3

4.	Task 4 Sensor Control Simulation:
nasm -f elf64 task_4.asm -o task_4.o
ld task_4.o -o task_4
./task_4

Insights and Challenges

1. Number Classification

	•	Insights: Efficient use of conditional (JE, JL) and unconditional (JMP) jumps simplifies control flow.
	•	Challenges: Ensuring branching logic covers all cases without redundancy.

2. Array Reversal

	•	Insights: Efficient two-pointer logic facilitates in-place array manipulation.
	•	Challenges: Managing precise memory index calculations to avoid errors.

3. Factorial Calculation

	•	Insights: Modular design with subroutines enhances code reusability and clarity.
	•	Challenges: Accurate stack management for preserving registers and handling edge cases like 0!.

4. Sensor Control Simulation

	•	Insights: Provides a practical demonstration of real-world sensor logic.
	•	Challenges: Safely manipulating memory while implementing multi-threshold control logic.

This repository is licensed under the MIT License. See the LICENSE file for more details.
