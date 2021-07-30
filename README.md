# OPL2LPT-Replica
## Introduction
This is a re-designed, open-source simple version of OPL2LPT circuit board with few components, acting as a YM3812 FM synthesizer on LPT port (***Adlib Card*** Compatible).

Buy the original version of OPL2LPT and for more info: https://www.serdashop.com/OPL2LPT.

## Development & Manufacture
- Please use ***Altium Designer 16*** or above to open or edit the PCB project

- Gerber files and NC drill files are already exported. PCB samples can be easily manufactured

   https://www.jlc.com/ is recommended for ordering PCB samples in China

- Using 74LS04 (TTL) to substitutes 74HC04 (CMOS) for the clock generator is not recommended, and may causing the circuit's failure

- XTAL must be 3.58MHz for accurate pitch of notes

- Parameters for components are noted on the board's silkscreen. More info in the PCB project
## Notes for Testing
- 5V DC power is needed, either from Mini-USB or external power pins
- Manually reset (RST SW) is needed when YM3812 behaves abnormal
- Available open-source drivers for this project:
  - on MS-DOS: https://github.com/pdewacht/adlipt (working fine using either method below)
    - Using TSR  `adlipt`  for port mapping (with emm386.exe)
    - Using  `adpatch`  to patch some DOS games
  - on Windows 3.1: https://github.com/andreiw/adlib21 (without testing)
## License
MIT license is chosen for this project.
## Update
- Ver 0.1(beta):First PCB for debugging
- Ver 0.2(beta):
  - A smaller re-designed PCB
  - Audio quality improved
- Ver 0.3(beta):Fix unconnected GND net on 3.5mm audio jack
- Ver 1.0:
  - First version updated on https://github.com/
  - Fix power LED & volume control's problem
  - A round PCB corner for easier assembling (with a 3D-Printed case)
  - Pull-up resistors on bus are removed to improve compatibility for some PCs
  - Use non-SMT Mini-USB port, making it easier to solder by hand
  - Add external power pins
- Ver 1.0.1:
  - Add 3D-Printed case (with cover) and knob (thanks for **@zhblue** for your awesome *.stl models)
  - Update directory structure for GitHub repo
