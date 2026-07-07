# JK-FLIP-FLOP-CADENCE-VIRTUOSO
To design a CMOS JK Flip-Flop using Cadence Virtuoso.

Introduction- A JK Flip-Flop is a sequential digital circuit used for storing one bit of data. It is an improved version of the SR Flip-Flop because it eliminates the invalid input condition present in the SR Flip-Flop. The JK Flip-Flop changes its output only on the active edge of the clock signal and is widely used in counters, registers, frequency dividers, and memory circuits.

A CMOS JK Flip-Flop is implemented using complementary PMOS and NMOS transistors in Cadence Virtuoso to achieve low power consumption, high noise immunity, and reliable switching performance.

Objective
1. To design a CMOS JK Flip-Flop using Cadence Virtuoso.
2. To verify the functionality of the flip-flop through transient simulation.
3. To analyze the output waveform for different combinations of inputs J, K, and Clock.
4. To understand the operation of edge-triggered sequential circuits.

Software Used- Cadence Virtuoso, Cadence Spectre Simulator, Technology Library (GPDK 90 nm / 180 nm or as provided)

Components Used- PMOS Transistors, NMOS Transistors, Voltage Sources (VDD, Ground), Pulse Voltage, Sources (Clock, J, K Inputs), Wires and Pins, Capacitor (optional load)

Circuit Description- The JK Flip-Flop is constructed using CMOS logic gates and feedback connections. The circuit accepts two inputs (J and K), a clock signal, and produces complementary outputs Q and Q̅.
The output changes only during the triggering edge of the clock.
The four operating conditions are:
J = 0, K = 0: No Change
J = 0, K = 1: Reset
J = 1, K = 0: Set
J = 1, K = 1: Toggle

Working Principle-
1. When J = 0 and K = 0, the flip-flop retains its previous state.
2. When J = 0 and K = 1, the output is reset to logic LOW.
3. When J = 1 and K = 0, the output is set to logic HIGH.
4. When J = 1 and K = 1, the output toggles its previous state at every active clock edge.
5. The complementary output Q̅ is always the inverse of Q.

Simulation Procedure-
1. Create a new library and cell in Cadence Virtuoso.
2. Draw the JK Flip-Flop schematic using CMOS transistors.
3. Connect VDD and Ground.
4. Apply pulse inputs for J, K, and Clock.
5. Perform electrical rule checks.
6. Launch Spectre simulation.
7. Run transient analysis.
8. Observe the output waveforms for Q and Q̅.
9. Verify the output with the truth table.

Applications-
1. Binary Counters
2. Shift Registers
3. Frequency Dividers
4. Digital Clocks
5. Sequence Generators
6. Memory Devices
7. Finite State Machines (FSMs)

Advantages
1. No invalid input condition.
2. Can operate as SR, D, or T Flip-Flop with suitable input connections.
3. Reliable edge-triggered operation.
4. Low power consumption using CMOS technology.
5. High noise immunity.
6. Suitable for high-speed digital circuits.

Result- The CMOS JK Flip-Flop was successfully designed and simulated in Cadence Virtuoso. The simulation verified that the circuit correctly performs Set, Reset, Hold, and Toggle operations according to the applied inputs and clock signal, matching the expected truth table.
