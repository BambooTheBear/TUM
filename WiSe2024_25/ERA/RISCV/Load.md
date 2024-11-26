
| Instruction      | Description                                 | Operation                                 | Use                                                                                                                                                        | Notes   |
| ---------------- | ------------------------------------------- | ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| lb rd, imm(rs1)  | load byte                                   | rd = [[Sign Extension\|SignExt]](rs1+imm) | set the [[Register]] rd to the (byte-) value in the cell of the [[Hauptspeicher]] at the address rs1+imm                                                   | 8bit    |
| lh rd, imm(rs1)  | load half                                   | rd = [[Sign Extension\|SignExt]](rs1+imm) | ^^ with 16bit (2byte)                                                                                                                                      | 16bit   |
| lbu rd, imm(rs1) | load byte unsigned                          | rd = [[ZeroExtension\|ZeroExt]](imm)      | ^^ with 8bit, but extends the missing 24bits with 0, not keeping the sign                                                                                  | 8bit    |
| lhu rd, imm(rs1) | load half unsigned                          | rd = [[ZeroExtension\|ZeroExt]](imm)      | ^^ with 16bit, extension with 0                                                                                                                            | 16bit   |
| lw rd, imm(rs1)  | load word                                   | rd = [[Sign Extension\|SignExt]](rs1+imm) | used to load the entire value (32bit/4byte) of the cell at rs1+imm                                                                                         | 32bit   |
| lui rd, upimm    | load upper <br>immidiate                    | rd = upimm_12\*b0                         | Used to load an entire 32 bit immidiate value by using _lui_ with the 20 most significant bits<br>and then adding the lower 12bits with _addi rd, rd, imm_ | 20bit   |
| li rd, imm       | [[Pseudo Instruction]] <br>"load immidiate" | rd = imm                                  | Loads an entire 32-bit immidiate into rd, **often not included in instruction set, lui/addi safer!!**                                                      | "32bit" |

^c44fab

