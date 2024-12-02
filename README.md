Digital Communication System Design
Instructor
Hafsa Batool

Teaching Assistants
Rimsha Ashfaq
Muhammad Ahmad
Moeed Ahmad
Date of Submission
1st December 2023

Overview
This project implements a Digital Communication System that transmits and receives data using a counter-based methodology. The system utilizes shift-left operations, logic gates (NOT, AND), and counters to ensure accurate data transmission between the transmitter and receiver. The design ensures efficient, precise, and synchronized communication.

Design Components
Transmitter Design
Counter-Controlled Operation:

The transmitter's functionality is managed by the third output (Q2) of a counter.
A NOT gate is employed to stop the counter when Q2 reaches the binary value 100 (4 in decimal).
This halts the transmission process after a complete cycle, ensuring data accuracy.
Data Loading:

Input values are loaded into the transmitter using a switch:
Switch = 0: Input values are loaded.
Switch = 1: The clock starts, initiating value shifting based on the setup.
Shift Left Operation:

A NOT gate ensures that data shifts in the reverse direction when linked to the switch.
The "Shift Left" operation is central to controlled output transitions within the transmitter.
Transmission Halt:

An AND gate takes the clock and the NOT value of Q2 as inputs.
This halts the transmitter when the counter reaches the state 100, stopping further data transmission.
Receiver Design
Architecture:

The receiver design closely mirrors the transmitter, incorporating similar components and functionalities.
Shift Left with Transmitter Output:

The receiver’s shift-left operation leverages the final output of the transmitter.
This ensures the received data (binary 0 or 1) is shifted appropriately.
Reconstruction of Data:

The receiver accurately reconstructs the original input data transmitted by the transmitter.
Features
Efficient Data Transmission: The counter-based approach ensures seamless communication with controlled data shifts.
Precise Halting Mechanism: Integration of counters and logic gates halts processes at predefined states, ensuring no data loss or corruption.
Symmetric Design: Identical architecture for transmitter and receiver simplifies implementation and ensures compatibility.
How to Use
Set Up:

Connect the system components, including counters, gates, and switches, as per the transmitter and receiver designs.
Load Data:

Set the switch to 0 to load input data into the transmitter.
Transmit Data:

Flip the switch to 1 to start the clock and initiate data shifting.
Receive Data:

The receiver will reconstruct the transmitted data using its shift-left operation.
Potential Improvements
Implement error detection and correction mechanisms for robust communication.
Add a visualization module to monitor data transfer and reconstruction in real-time.
Expand to support multi-bit parallel data transfer.
Acknowledgment
This project was guided by Instructor Hafsa Batool and supported by TAs Rimsha Ashfaq, Muhammad Ahmad, and Moeed Ahmad.
