(all 32bit / 4 Byte)

| zero  | x0     | Always 0                                    |
| ----- | ------ | ------------------------------------------- |
| ra    | x1     | Return address                              |
| sp    | x2     | Stack Pointer => use like "0(sp), 4(sp)..." |
| gp    | x3     | Global Pointer                              |
| tp    | x4     | Thread pointer                              |
| t0-2  | x5-7   | Temporary registers                         |
| s0/fp | x8     | Saved Register 0 / (Frame Pointer?)         |
| s1    | x9     | Save Register 1                             |
| a0-1  | x10-11 | Function Arguments & Return Values          |
| a2-7  | x12-17 | additional Function arguments               |
| s2-11 | x18-27 | Saved Register                              |
| t3-6  | x28-31 | Temporary registers                         |
