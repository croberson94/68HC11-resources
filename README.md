# 68HC11 Microcontroller
A collection of resources for the 68HC11 microcontroller. In particular, this guide will focus on the CME11E9-EVBU version of this development board. If there are any updates you would like to contribute, submit a pull request!

## Availability
This board is available from [Axiom Manufacturing](https://www.axman.com/content/cme-11e9-evbu-single-chip-expanded-mode-development-system-mc68hc11e9-32k-sram-8k-eeprom) .

## Documentation
### General Manufacturer Information
* [Axman CME-11E9-EVBU](https://www.axman.com/content/cme-11e9-evbu)
* [Jameco M68HC11E Family Data Sheet](https://www.jameco.com/Jameco/Products/ProdDS/248575MOT.pdf)

### Other Information
* [68HC11 Instruction Set](http://dankohn.info/projects/68HC11/68HC11%20Instruction%20Set.htm)
* [Motorola S19 File Format](https://www.x-ways.net/winhex/kb/ff/Motorola-S3.txt)

## Environments
The main compilation environment is DOSBox, using the AS11 assembler (see below).
* [DOSBox](https://www.dosbox.com)
* [DOSBox Tutorial](https://www.dosbox.com/wiki/Basic_Setup_and_Installation_of_DosBox)

## Communication with Board
The methods used to communicate with the development board differ on Windows and Mac/Linux.

### Windows
Download and install [Tera Term](https://osdn.net/projects/ttssh2/releases/). Connect to the board using the default parameters--9600 baud, 1 stop bit, no parity. Proceed using Buffalo Monitor.

### Mac/Linux
Utilize `screen`, a terminal multiplexer, which has built in serial communication capabilities. This should be installed by default on all Mac and Linux machines. Read the instructions at [http://www.noah.org/wiki/Screen_notes#using_screen_as_a_serial_terminal](http://www.noah.org/wiki/Screen_notes#using_screen_as_a_serial_terminal) for more information.

## Emulators
*  [THRSim11](http://www.hc11.demon.nl/thrsim11/thrsim11.htm)

## Interface
The operating system for the M68HC11 is the Buffalo Monitor.
* [Buffalo Monitor OS](https://www.mil.ufl.edu/projects/gup/docs/buffalo.pdf)

The main assembler for the source code is as11, for the Axiom development environment (AxIDE).
* [AxIDE compiler](https://www.axman.com/content/axide)

MGTEK MiniIDE provides much of the functionality of the Axiom IDE with the addition of syntax highlighting.
* [MGTEK MiniIDE](https://www.mgtek.com/miniide/)

## Disassembly, Code-Recovery, Reverse-Engineering, and Code-Analysis
GenDasm, the Generic Code-Seeking Disassembler engine with Fuzzy-Function Analyzer, uses a DNA Sequence Alignment Algorithm to locate similar code in multiple binaries to facilitate reverse-engineering and/or code recovery.  It's also useful to analyze compiler code-generation and help with making optimizations.
* [Generic Code-Seeking Disassembler with Fuzzy-Function Analyzer](https://github.com/dewhisna/gendasm)

ASxxxx Cross-Assemblers by Alan Baldwin at Kent State University.
* [ASxxxx Cross-Assemblers](https://shop-pdp.net/index.php) and specifically the [AS6811 Assembler](https://shop-pdp.net/ashtml/as6811.htm), is targeted by GenDasm to reassemble (or roundtrip) disassembled code back to the original binary.

## Virtualization
* [VirtualBox](https://www.virtualbox.org/)

## Text Editors
Recommended text editors for source code:
* [Notepad++](https://notepad-plus-plus.org)
* [Vim](https://www.vim.org)  
* [MacVim](https://macvim-dev.github.io/macvim/)
