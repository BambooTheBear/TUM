
| Instruction       | Description                          | Operation                                   | Use                                         | Notes                               |
| ----------------- | ------------------------------------ | ------------------------------------------- | ------------------------------------------- | ----------------------------------- |
| addi rd, rs1, imm | add immidiate                        | rd = rs1 + [[Sign Extension\|SignExt]](imm) | _load a constant with addi rd, zero, 0x12c_ | imm can be at most 12 bits          |
| add rd, rs1, rs2  | addition of 2 values in registers    | rd = rs1 + rs2                              |                                             | addition with neg. numbers possible |
| sub rd, rs1, rs2  | subtraction of 2 values in registers | rd = rs1 - rs2                              |                                             | no "subi" available                 |
