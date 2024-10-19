# reversing-notes

## GDB stuff

### Run program with no extensions
`gdb --nx <binary>`

`info functions`

`info registers`

`disassemble <function name>`

### Strip debugging symbols from binary
`strip <binary>`

Stack frame -- one per function
retq -- "q" for quad-word, meaning 64-bit instead of 32-bit
