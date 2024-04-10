# Ghidra processor description module for NEC/Renesas v810 and v830 families
1. V810 version based on **User’s Manual: V810 Architecture** ([link](https://files.virtual-boy.com/download/978644/u10082ej1v0um00.pdf))
2. V830 version based on **User’s Manual: V830 Architecture** ([link](https://www.renesas.com/us/en/document/mat/v830tm-hardware))
## Installation

1. Compile the SLEIGH CPU descriptions with:

`$(GHIDRA_HOME)\support\sleigh.bat data\languages\V810.slaspec`

`$(GHIDRA_HOME)\support\sleigh.bat data\languages\V830.slaspec`

2. Copy the `V800` folder to:
`$(GHIDRA_HOME)\Ghidra\Processors\`
## TODOs
### V830

### V810
Determine e_machine value in .ELF files, if any.
Implement

