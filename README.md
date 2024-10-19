# reversing-notes

## GDB stuff

### Run program with no extensions
`gdb --nx <binary>`

### Change to intel disassembly syntax rather than gdb default AT&T
`set disassembly-flavor intel`

`info functions`

`info registers`

`disassemble <function name>`

### Disassemble with opcodes
`disassemble /r <function name>`

### Setting breakpoints
Offset 4 from within main function (gdb displays these as e.g. <+4>)
`break *main+4`

Examine instruction (x/i) at $rip (the instruction pointer)
`x/i $rip`

Examine memory as a string (x/s) an address
`x/s $rip+0xec4`
`x/s 0x55555555`

### Strip debugging symbols from binary
`strip <binary>`

Stack frame -- one per function
retq -- "q" for quad-word, meaning 64-bit instead of 32-bit
