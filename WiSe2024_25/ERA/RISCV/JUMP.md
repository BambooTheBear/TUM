PC = [[ProgrammCounter]]

| Instruction      | Description                   | Operation                                              | Use                                                                                                                                                                           | Notes                            |
| ---------------- | ----------------------------- | ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| jalr rd, rs, imm | jump and link register        | rd = PC+4;<br>PC = rs+[[Sign Extension\|SignExt]](imm) | _Jumps_ to the instruction in the instruction-stack at rs+imm (_Register_ +imm)<br>and _links_ the next instruction into rd => saves the _return address_ usually into **ra** | usually only for <br>quick jumps |
| jal rd, label    | jump and link (label)         | rd = PC+4;<br>PC = label                               | ^^ as above but jump to a label (call a function by the "function-name")                                                                                                      | proper instruction <br>for calls |
| jal label        | [[Pseudo Instruction]]        | jal ra, label                                          | just like jal but since the return address ist almost always in **ra** (because [[Convention]]) this is just shorter                                                          | used most                        |
| j label          | [[Pseudo Instruction]] Jumpr  | jal zero, label                                        | jumpt to a function without storing (or overwriting) the return address                                                                                                       |                                  |
| ret              | [[Pseudo Instruction]] return | jalr zero, ra, 0                                       | jumps to the stored return address (without saving a "new" return address obv.)                                                                                               | easy return                      |
