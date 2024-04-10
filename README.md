# Ghidra processor description module for NEC/Renesas v810 and v830 families
These modules were made by taking the v850 modules that come with Ghidra as a template and rewriting them to work with v810 and v830 family instructions.
1. V810 description based on **User’s Manual: V810 Architecture** ([link](https://files.virtual-boy.com/download/978644/u10082ej1v0um00.pdf))
2. V830 description based on **User’s Manual: V830 Architecture** ([link](https://www.renesas.com/us/en/document/mat/v830tm-hardware))
## Installation

1. Compile the SLEIGH CPU descriptions with:

`$(GHIDRA_HOME)\support\sleigh.bat data\languages\V810.slaspec`

`$(GHIDRA_HOME)\support\sleigh.bat data\languages\V830.slaspec`

2. Copy the `V800` folder to:
`$(GHIDRA_HOME)\Ghidra\Processors\`
## Hardware Documentation
Some CPUs, such as the v831, come with built-in peripherals (i.e. DMA controller, UART, CSI, Timers, etc.). Therefore, if hardware documentation for a CPU in these families is available (with or without peripherals), they will be listed below:
### v810 Family
**User's Manual: V805, V810 Hardware** ([link](http://goliathindustries.com/vb/download/cpu/U10661EJ5V0UM00.pdf))

(V820's existence is alluded to in various manual documents but no datasheets nor manuals have been found at this moment.)

**User’s Manual: V821 Hardware** ([link](https://www.renesas.com/us/en/document/mah/v821tm-hardware))
### v830 Family
 **User’s Manual: V830 Hardware** ([link](https://www.renesas.com/us/en/document/mat/v830tm-hardware))

 **User’s Manual: V831 Hardware** ([link](https://www.renesas.com/us/en/document/mat/v831tm-hardware))

 **User’s Manual: V832 Hardware (Preliminary)** ([link](https://www.renesas.com/us/en/document/mah/v832tm-hardware-preliminary))
## TODOs
### v830
Add .idx for instruction documentation.

Cleanup.

### v810
Determine e_machine value in .ELF files, if any.

Implement bit string instructions.

Add .idx for instruction documentation.

