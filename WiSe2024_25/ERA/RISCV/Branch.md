used as a "conditional" [[JUMP]], but only to labels and never stores the return address.
To conditionally jump to non-label-adresses or to store the return address: branch to a seperate label with the actual jump to the function/label

| Instruction       | Description                   | Operation        | Use                                                                             | Notes       |
| ----------------- | ----------------------------- | ---------------- | ------------------------------------------------------------------------------- | ----------- |
| beq r1, r2, label | branch if equal               | _r1=r2_ ?        | Jumps to the label if the value in r1 is equal to the value in r2               | ==          |
| bne r1, r2, label | branch if NOT equal           | _r1!=r2_ ?       | Jumps to the label if the value in r1 is NOT equal to the value in r2           | !=          |
| blt r1, r2, label | branch if less then           | _r1<r2_ ?        | Jumps to the label if the value in r1 is smaller than the value in r2           | <           |
| bge r1, r2, label | branch if greater or equal    | _r1>=r2_ ?       | Jumps to the label if the value in r1 is greater or euqal to the value in r2    | >=          |


