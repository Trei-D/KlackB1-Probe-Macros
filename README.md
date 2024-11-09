# Biqu B1 Klack Probe Macros Installation Guide

## Overview
This guide will help you install and configure the Klack Probe Macros modification for your Biqu B1 3D printer, integrating it with Demon Klipper Essentials Unified.

## Prerequisites
- All printed parts from the [STL directory](https://github.com/Trei-D/Biqu-B1-Klack-Probe/tree/main/STL)
- Required hardware components ([See BOM](https://kevinakasam.com/klack-bom/))
- Klipper firmware installed and operational
- Basic understanding of Klipper configuration

## Hardware Installation
Complete hardware assembly instructions can be found in the [Biqu B1 Klack Probe Repository](https://github.com/Trei-D/Biqu-B1-Klack-Probe/tree/main).

### Assembly Checklist
- [ ] Print all required components
- [ ] Gather hardware from BOM
- [ ] Install probe mount
- [ ] Install probe dock
- [ ] Verify mechanical operation

## Software Configuration

### 1. Installing Demon Klipper Essential Unified

1. Install the base package:
   ```bash
   # Clone the repository
   git clone https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified.git
   ```

2. Follow the [Klicky Probe setup instructions](https://github.com/3DPrintDemon/Demon_Klipper_Essentials_Unified/blob/main/Documentation/INSTALL_INSTRUCTIONS/General%20_Setup_For_All_Printers/INSTALL_INSTRUCTIONS.md#unless-youre-using-klicky-probe)

### 2. KlackB1-Probe Macro Setup

1. Create the KlackB1 directory:
   ```bash
   # Navigate to your Klipper config directory
   cd ~/printer_data/config
   
   # Create new directory
   mkdir KlackB1
   ```

2. Copy probe macros:
   ```bash
   # Copy macros from this repository to KlackB1 folder
   cp /path/to/repository/macros/* ~/printer_data/config/KlackB1/
   ```

3. Update your `printer.cfg`:
   ```yaml
   [include KlackB1/klicky-probe.cfg]
   ```

## Verification Steps

After installation, verify:
1. All mechanical components move freely
2. Probe attaches and detaches correctly
3. Probe triggers consistently
4. Macros execute without errors

## Troubleshooting

Common issues and solutions:
- Probe not attaching: Check dock alignment
- Probe not triggering: Verify wiring and pin configuration
- Macro errors: Check config file syntax

## Contributing

Found a bug or want to contribute? Please:
1. Open an issue describing the problem or enhancement
2. Submit pull requests with clear descriptions
3. Follow the project's coding standards

## License

This modification is released under the same license as the original KlackEnder-Probe project.

---
Last updated: November 2024