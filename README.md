# UART-Implementation-in-FPGA
Semester 04 - EN2111 Electronic Circuit Design

This repository contains the Verilog implementation of a full-duplex Universal Asynchronous Receiver-Transmitter (UART) designed for FPGA. This project was developed as part of the EN2111 FPGA Assignment at the University of Moratuwa. 🎓

📋 Project Overview
The UART transceiver is a parameterized, full-duplex module that utilizes dedicated finite state machines (FSM) for serial data transmission and reception. It adheres to standard RS-232 specifications, featuring:

⚙️ Parameterized Baud Rate: Internally generated 115200 baud rate using counters derived from the system clock.

✅ Robust Framing: Proper start/stop bit framing and LSB-first data transfer.

⚡ Asynchronous Stability: A double-flop synchronizer to prevent metastability on asynchronous inputs.

🎯 Accurate Data Recovery: Implements middle-of-bit sampling.

🛠️ Implementation Details
Target Device: FPGA 🧊

Protocol: RS-232 standard 🔌

System Clock: 50 MHz ⏱️

Baud Rate: 115200 bps 📈

🔬 Hardware Functionality
The design was verified on hardware by transmitting an incrementing number (0-9).

Inputs: KEY0 for active-low reset, KEY1 for increment/transmit trigger.

Outputs: Received data is displayed on a 7-segment display, with the binary pattern shown on onboard LEDs. 💡

Verification: Hardware validation included both local loopback configurations and cross-board communication between two FPGAs. Oscilloscope measurements confirmed timing precision and signal integrity, with a measured bit width of ~8.7 µs, corroborating the 115200 baud rate. 📊

👥 Team Members (Group 37)

Weerakoon A.H.T.M. (230689A)

Weerasinghe J.A.H.R. (230697V)

Wijesekara W.A.G.S. (230724E)
