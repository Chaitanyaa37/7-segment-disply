# 7-Segment Display Counter using 8051 Microcontroller

This project demonstrates how to display digits 0 through 9 sequentially on a 7-segment display using an 8051 microcontroller. The code is written in embedded C and built using the Keil µVision IDE.

# Description

The microcontroller is programmed to output the correct segment values for each digit from 0 to 9. A delay is used between each digit to make the changes visible on the 7-segment display. The display is connected to Port 2 (P2) of the 8051.

# File Structure

- 7 segment.c: Source code written in C for the 8051.
- 7 segment.hex: Compiled hex file for flashing onto the microcontroller.
- 7 segment.uvproj: Keil µVision project file.

# Requirements

- Keil µVision IDE
- 8051 Development Board (e.g., AT89C51)
- 7-Segment Display
- Programmer/Flasher for 8051
- Jumper wires and breadboard

# Hardware Connections

Connect the 7-segment display to Port 2 of the 8051 (P2.0–P2.7). Common cathode display is assumed. Segment codes are directly written to P2 in the code.

# Working Logic

Each digit is represented by a unique hex value corresponding to the segments that need to be lit. These values are written to P2, with a small delay in between:
