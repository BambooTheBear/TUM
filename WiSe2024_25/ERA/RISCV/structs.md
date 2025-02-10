To use "structs" or "class-Objects" in RISCV, we use _labels_
```
example:
	.word // =int => 4 Byte
	.short // =short => 2 Byte
	.word  // =int => 4 Byte
	.byte // =char => 1 Byte

la a0, example // pseudo Instruction "load address" of a label into a0
li t0, 12 // load some value into t0
sw t0, 6(a0) // save our t0 into "The registers that come after the first 6 (4+2) Bytes of the address in the label" => store t0 into the second int of example
```
