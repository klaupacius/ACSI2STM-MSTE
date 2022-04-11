# ACSI2SD-MSTE
 
This a KiCAD (6.0) design to host an [ACSI2STM](https://github.com/retro16/acsi2stm) directly inside an Atari Mega STE using the internal connector. 
The PCB has been designed to accomodate version 2.43 of ACSI2STM (aka V2) but also the V1 design as sold by @masteries on AtariAge. 
- No external power is required, the 5v is taken directly from the internal ACSI connector, but this has only been tested with a fully recapped PSU. 
- A set of jumper needs to be soldered to configure the board for V1 or V2 as noted on the PCB.

:warning: **DO NOT PLUG ANY USB CABLE ON THE STM32 ONCE INSTALLED IN THE MEGA STE** :warning:

![ACSI2STM Adapter render](https://github.com/olivierjan/ACSI2SD-MSTE/blob/main/ACSI2SD%20MSTE.png)

## BOM
- 100 nF Capacitor
- 10uF Radial Capacitor
- Female 2.54 headers
- Amphenol GSD090012SEU SD Card socket
- STM32F103C8T6 "Blue Pill" (original one is highly recommended!!!). 
- Firmware from [ACSI2STM](https://github.com/retro16/acsi2stm) or from @masteries. 

## Configuration
Configuration is done by simple solder bridges on the pads, instructions are also written on PCB.

### For V1:
- Solder bridge: JP1, JP2, JP3, JP4, JP5, JP6, JP7
- Solder bridge pads 1 and 2 of JP9 (2 leftmost pads)
- Solder bridge pads 1 and 2 of JP10 (2 leftmost pads)

### For V2: 
- Solder bridge pads 2 and 3 of JP9 (2 leftmost pads)
- Solder bridge pads 2 and 3 of JP10 (2 leftmost pads)
- Solder bridge JP8 (optional but recommended)

:warning: **DO NOT PLUG ANY USB CABLE ON THE STM32 ONCE INSTALLED IN THE MEGA STE** :warning:
