# Installation Guide

## Prerequisites
- Printed parts
- Required hardware (see [BOM.md](https://kevinakasam.com/klack-bom/))
- Klipper firmware installed

## Hardware
[Biqu B1 Klack Probe](https://github.com/Trei-D/Biqu-B1-Klack-Probe/tree/main)


## Software Setup
Demon Klipper Essential Unified + KlackB1-Probe Macros

1.1. Install [Demon_Klipper_Essentials_Unified](https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/tree/main) by following the instructions from the repository.

1.2. Be sure to follow the instructions from this [step](https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/blob/main/Documentation/INSTALL_INSTRUCTIONS/General%20_Setup_For_All_Printers/INSTALL_INSTRUCTIONS.md#unless-youre-using-klicky-probe) 

1.3. Create a new directory in config folder with the name KlackB1

1.4. Copy the macros from this repository into KlackB1 folder

1.5. Edit printer.cfg by adding this line [include KlackB1/klicky-probe.cfg]
