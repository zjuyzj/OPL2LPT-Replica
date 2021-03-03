# OPL2LPT-Replica
## Introduction
<img src=".\OPL2LPT Replica v0.2.jpg" alt="OPL2LPT Replica v0.2" style="zoom: 20%;" />

This is a re-designed and open-source OPL2LPT circuit board with really few components, acting as a YM3812 FM synthesizer on LPT port(Adlib compatible, work fine with `adlipt` TSR and DOS games under `adpatch`).

Buy the original version of OPL2LPT and for more info: https://www.serdashop.com/OPL2LPT.

## Development&Manufacture
- Please use Altium Designer 16 or above to open&edit the PCB project.
- Gerber files and NC drill files are already exported. PCB samples can be easily manufactured. https://www.jlc.com/ is recommended for ordering PCB samples.
- Using 74LS04(TTL) to substitutes 74HC04(CMOS) for the clock generator is not recommended(and may causing the circuit's failure).
- XTAL must be 3.58MHz for accurate pitch of notes.
- Parameters for components are noted on the board's silkscreen. More info in the PCB project.  
## Notes for Testing
- 5V DC power is needed, either from Mini-USB or external power pins.

- Manually reset(RST SW) is needed when YM3812 behaves abnormal.

- Available open-source drivers for this project on MS-DOS(with emm386.exe): https://github.com/pdewacht/adlipt and watch it for more details. Windows driver is under development in `./softwares` directory.
## License
MIT license is chosen for this project.
## Update
- Ver 0.1(beta):First PCB for debugging.
- Ver 0.2(beta):
  - A smaller re-designed PCB. 
  - Audio quality improved.
- Ver 0.3(beta):Fix unconnected GND net on 3.5mm audio jack.
- Ver 1.0:
  - First version updated on https://github.com/.
  - Fix power LED & volume control's problem.
  - A round PCB corner for easier assembling(with a 3D printed case).
  - Pull-up resistors on bus are removed to improve compatibility for some PCs.
  - Use non-SMT Mini-USB port,making it easier to solder by hand.
  - Add external power pins.
