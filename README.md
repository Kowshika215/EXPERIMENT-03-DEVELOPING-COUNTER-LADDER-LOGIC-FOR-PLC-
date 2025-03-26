# EXPERIMENT-03-DEVELOPING-COUNTER-LADDER-LOGIC-FOR-PLC-
## NAME: Kowshika.R
## REGISTER NUMBER: 212224220049
## DEPARTMENT: IT
## YEAR: I

### Aim:
To understand and implement various counter operations in Programmable Logic Controller (PLC) ladder logic.

### Apparatus Required:
Programmable Logic Controller (PLC): A PLC that supports counter functions.
PLC Programming Software: Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System: For programming and simulating the PLC ladder logic.
Input Devices: Push buttons or switches to trigger the counter operations.
Output Devices: LEDs or other indicators to visualize the counter outputs.
Wires and Connectors: For interfacing input/output devices with the PLC.
Power Supply: Appropriate power supply for the PLC and peripherals.

### Theory:
Counters in PLCs are used to count events or occurrences, such as the number of items passing on a conveyor belt, the number of cycles a machine runs, or how many times a process has started or stopped. Counters are commonly used in automation to perform tasks like stopping a machine after a set number of products or signaling a notification when a count reaches a specific value.

### Types of Counters:
Up Counter (CTU) Functionality:

The up counter counts every time the input condition becomes TRUE (ON). When the accumulated value reaches the preset value, the counter output becomes TRUE. If the reset input is triggered, the counter resets to zero.
Down Counter (CTD) Functionality:

The down counter decreases the count every time the input condition becomes TRUE (ON). When the count reaches zero, the counter output becomes TRUE. The counter can be reset by a reset input to the preset value.
Up/Down Counter (CTUD) Functionality:

The up/down counter can increment or decrement the count based on two different inputs. One input increments the count, while the other decrements it. When the count reaches the preset value or zero, the respective outputs become TRUE. The counter can be reset as required.


### Procedure:
Setup the PLC Programming Environment:
Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Counters:
Up Counter (CTU):

Create a rung with an input (e.g., a push button) linked to a CTU instruction.
Set the preset value (e.g., 10 counts). Assign an output to indicate when the preset value is reached.
Down Counter (CTD):

Create a rung with an input linked to a CTD instruction.
Set the preset value (e.g., 5 counts). Assign an output to indicate when the counter reaches zero.
Up/Down Counter (CTUD):

Create a rung with separate inputs for counting up and counting down.
Set the preset value (e.g., 8 counts). Assign outputs for when the count reaches the preset value or zero.
Simulate the Ladder Logic:
Up Counter (CTU):

Run the simulation in the PLC software. Press the input button repeatedly and observe the counter increment until the preset value is reached, at which point the output activates.
Down Counter (CTD):

Run the simulation, press the input button repeatedly, and observe the counter decrement. When the counter reaches zero, the output activates.
Up/Down Counter (CTUD):

Simulate both the up and down counting inputs. Observe how the counter increments or decrements and how the output is activated when the count reaches the preset value or zero.
Download and Execute:
Download the ladder logic program to the PLC if available and run it.
Test the counters with the physical push buttons and observe the LEDs or other output devices.
### Outputs:
Up Counter (CTU): The output LED or indicator should activate when the preset count (e.g., 10) is reached.

Down Counter (CTD): The output should activate when the count reaches zero.

## PROBLEM STATEMENT:
Design PLC ladder logic that reads input from 2 sensors providing counting operation starting from 0 to 10. Also switch ON conveyer but reaching packet station and seal packet after 5s of delay.

### Simulation Screenshots:

COUNTER UP:

![Screenshot 2025-03-26 132108](https://github.com/user-attachments/assets/7214f0dd-3fe4-45bc-ac4a-13c4f3046c1b)

COUNTER DOWN:

![WhatsApp Image 2025-03-25 at 19 01 07_7cae0741](https://github.com/user-attachments/assets/a43aaefb-9113-4cc2-988a-b77cdf735a0a)

PROBLEM STATEMENT:
Device a PLC lader logic that can read data from two sensors providing the counting operation starting from 0 to 10 and switch on 
convirment reaching the packet station and seal the packet station and seal the packet after 5sec of delay.

COUNTER UP:

![WhatsApp Image 2025-03-25 at 19 01 08_0601e573](https://github.com/user-attachments/assets/6d2ae8e4-fd2a-40a0-839e-db175b9cca5a)

COUNTER DOWN:

![WhatsApp Image 2025-03-25 at 19 01 09_26207b2a](https://github.com/user-attachments/assets/73db210a-4e78-4d0c-a072-32f5183b314c)


### Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
