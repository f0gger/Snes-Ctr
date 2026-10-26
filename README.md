# SNES Controller – KiCad Hardware Design

KiCad hardware design files for a custom Super Nintendo Entertainment System (SNES) controller built around the ATmega328P microcontroller, with I²C communication for interfacing with external devices.

## Repository Structure

```text
Snes-Ctr/
├── gerbers/ - Gerber and drill files for PCB manufacturing.
│   ├── Snes-Ctr-B_Cu.gbl
│   ├── Snes-Ctr-B_Mask.gbs
│   ├── Snes-Ctr-B_Paste.gbp
│   ├── Snes-Ctr-B_Silkscreen.gbo
│   ├── Snes-Ctr-Edge_Cuts.gm1
│   ├── Snes-Ctr-F_Cu.gtl
│   ├── Snes-Ctr-F_Mask.gts
│   ├── Snes-Ctr-F_Paste.gtp
│   ├── Snes-Ctr-F_Silkscreen.gto
│   ├── Snes-Ctr-NPTH.drl
│   ├── Snes-Ctr-PTH.drl
│   └── Snes_Ctr_gerbers.zip
├── Snes-Ctr.kicad_dru - Custom PCB design rules
├── Snes-Ctr.kicad_pcb - PCB layout.
├── Snes-Ctr.kicad_pro - KiCad project configuration.
├── Snes-Ctr.kicad_sch - Circuit schematic.
└── README.md
```

File names and structure may vary depending on the actual project files.
Hardware Overview

The controller uses the ATmega328P to interface with the SNES controller inputs and handle communication with external hardware over the I²C bus.

The KiCad project contains the circuit schematic and PCB design, providing a starting point for reviewing, modifying, and manufacturing the hardware.
Requirements

    KiCad — for viewing and editing the schematic and PCB
    ATmega328P-compatible programming hardware — for flashing firmware, if applicable

## Getting Started

    Clone this repository:
    ```bash
    
    git clone <repository-url>
    cd <repository-directory>
    ```
    
    Open the .kicad_pro file in KiCad.
    Review the schematic (.kicad_sch) to understand the circuit.
    Open the PCB editor to inspect or modify the board layout.
    Run the electrical rules check (ERC) and design rules check (DRC) before manufacturing.

## Manufacturing

Before ordering or assembling the PCB:

    - Verify the schematic and PCB design.
    - Check component footprints and pin assignments.
    - Run ERC and DRC in KiCad.
    - Generate Gerber files and drill files using KiCad's fabrication tools.
    - Confirm the bill of materials (BOM) and component availability.
