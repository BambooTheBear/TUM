
| Instruction      | Description | Operation      | Use                                                                                                                                                      | Notes |
| ---------------- | ----------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| sb rs2, imm(rs1) | store byte  | \[rs1+imm]=rs2 | set the last byte (8bit) of the cell at the address _rs1+imm_ in the [[Hauptspeicher]]<br>to the (last byte of the) value stored in the [[Register]] rs2 | 8bit  |
| sh rs2, imm(rs1) | store half  | \[rs1+imm]=rs2 | ^^ with 16bit (2byte)                                                                                                                                    | 16bit |
| sw rs2, imm(rs1) | store word  | \[rs1+imm]=rs2 | ^^ with 32bit, so full register value overwrites full value in the Hauptspeicher                                                                         | 32bit |

^801857

