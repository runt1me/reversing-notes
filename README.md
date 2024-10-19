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

### Strip debugging symbols from binary
`strip <binary>`

Stack frame -- one per function
retq -- "q" for quad-word, meaning 64-bit instead of 32-bit
