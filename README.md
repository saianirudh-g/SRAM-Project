📘 6T SRAM Cell – Schematic, Simulation & Layout
This repository contains the schematic design, transient simulations, butterfly curve analysis, and layout implementation of a standard 6‑Transistor (6T) SRAM cell.

📐 1. Schematic Design
The 6T SRAM cell consists of:

2 cross‑coupled inverters (storage nodes Q and QB)

2 NMOS access transistors (controlled by WL)

Bit‑lines BL and BLB for read/write operations

The schematic is designed using standard CMOS design rules.

📊 2. Output Plots
2.1 Transient Response
Shows the dynamic behavior of the SRAM cell during:

Write ‘0’ / Write ‘1’ operations

Hold mode

Read operation

Includes waveforms for:

Q

QB

WL

BL / BLB

2.2 Butterfly Curve (Static Noise Margin)
The Butterfly Plot (QB vs Q) is generated to evaluate the Static Noise Margin (SNM).

Includes:

Cross‑coupled inverter VTC curves

Maximum square fitting method

SNM extraction line

This plot verifies the stability of the SRAM cell during read and hold operations.

🧱 3. Layout Design
The 6T SRAM layout is implemented following:

DRC‑clean design

Minimum spacing and width rules

Shared diffusion for inverter pairs

Poly‑gate alignment for matched transistors

Metal routing for WL, BL, BLB

Contact/via placement for stable connections

The layout includes:

PMOS and NMOS transistor placement

Wordline (WL) routing

Bitline (BL/BLB) routing

Storage nodes (Q, QB)

Well taps and substrate contacts

📁 Repository Structure (Suggested)
Code
├── schematic/
│   ├── 6T_SRAM_Schematic.png
│   └── netlist.sp
├── simulations/
│   ├── transient_response.png
│   ├── butterfly_curve.png
│   └── snm_extraction.png
├── layout/
│   ├── 6T_SRAM_Layout.png
│   └── drc_report.txt
└── README.md
