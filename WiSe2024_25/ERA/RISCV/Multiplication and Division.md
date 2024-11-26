
| Instruction         | Description                     | Operation       | Use                                                                                                  | Notes           |
| ------------------- | ------------------------------- | --------------- | ---------------------------------------------------------------------------------------------------- | --------------- |
| mul rd, rs1, rs2    | multiply                        | rd = rs1 \* rs2 | multiply rs1 with rs2, since 32bit\*32bit=64bit, this saves the <br>lowest 32 bits of the end result | sign irrelevant |
| mulh rd, rs1, rs2   | multiply high signed signed     | rd = rs1 \* rs2 | ^^ but stores the highest 32bit, so **full result is "mulh.mul"**                                    | both signed     |
| mulhsu rd, rs1, rs2 | multiply high signed unsigned   | rd = rs1 \* rs2 | like mulh but rs2 is an unsigned 32bit-integer                                                       | signed/unsigned |
| mulhu rd, rs1, rs2  | multiply high unsigned unsigned | rd = rs1 \* rs2 | like mulh but both are unsigned 32bit-integer                                                        | both unsigned   |

^b0332c

### Division
| Instruction       | Description     | Operation    | Use | Notes                  |
| ----------------- | --------------- | ------------ | --- | ---------------------- |
| div rd, rs1, rs2  | divide (signed) | rd = rs1/rs2 |     | always rounds **down** |
| divu rd, rs1, rs2 | divide unsigned | rd = rs1/rs2 |     |                        |
### Modulo (Remainder)

| Instruction       | Description         | Operation    | Use                                                     | Notes                                         |
| ----------------- | ------------------- | ------------ | ------------------------------------------------------- | --------------------------------------------- |
| rem rd, rs1, rs2  | remainder (signed)  | rd = rs1%rs2 | useful to see if two numbers are divisible => rem == 0? | $rs_1 - (\lfloor{(rs_1 / rs_2)}\rfloor*rs_2)$ |
| remu rd, rs1, rs2 | remainder unsigned) | rd = rs1%rs2 |                                                         |                                               |
