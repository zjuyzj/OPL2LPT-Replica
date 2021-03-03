# OPL2LPT-Replica
## Introduction
This is a re-designed and open-source OPL2LPT circuit board with really few components,acting as a YM3812 FM synthesizer on LPT port(Adlib compatible).
Buy the original version of OPL2LPT and for more info:`https://www.serdashop.com/OPL2LPT`.
## Development&Manufacture
- Please use Altium Designer 16 or above to open&edit the PCB project.
- Gerber files and NC drill files are already exported.PCB samples can be easily manufactured.`https://www.jlc.com/` is recommended for ordering PCB samples.
- Using 74LS04(TTL) to subtitudes 74HC04(CMOS) for the clock generator is not recommended(and may causing the circuit's failure).
- XTAL must be 3.58MHz for accurate pitch of notes.
## About Using
- 5V DC power is needed, either from Mini-USB or external power pins.
- Manually reset(RST SW) is needed when YM3812 behaves abnormal.
- Availble open-source drivers for this project on MS-DOS(with emm386):'https://github.com/pdewacht/adlipt' and watch it for more details.Windows driver is under development in `./softwares` directory.
##License
MIT license is chosen for this project.
## Update Logs
- Ver 0.1(beta):First PCB for debugging.
- Ver 0.2(beta):A smaller re-designed PCB.Audio quality improved.
- Ver 0.3(beta):Fix unconnected GND net on 3.5mm audio jack.
- Ver 1.0:
  - First version updated on github.
  - Fix power LED&volumn control's problem.
  - A round PCB conner for easier assembling(with a 3D printed case).
  - Pull-up resistors on bus are removed to improve compability for some PCs.
  - Use non-SMT Mini-USB port,making it easier to solder by hand.
  - Add external power pins.
