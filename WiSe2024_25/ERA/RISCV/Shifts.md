## Leftshifts
a shift left ("_b<<n_") shifts all the bits in _b_ by _n_ to the left, filling the rest with 0s
Called a **logical shift** because it fillst with 0s
⇒ This is just a multiplication by $2^n$, and it works for signed and unsigned

| Instruction        | Description                  | Operation        | Use                            | Notes                                                                  |
| ------------------ | ---------------------------- | ---------------- | ------------------------------ | ---------------------------------------------------------------------- |
| slli rd, rs1, uimm | shift left logical immidiate | rd = rs1\<\<uimm | multiplies rs1 with $2^{uimm}$ | uimm can be 20bits, but only 5bits are useful since $2^5=32$ => 32bits |
| sll rd, rs1, uimm  | shift left logical           | rd = rs1\<\<rs2  | multiplies rs1 with $2^{rs2}$  | **only the last 5bits of rs2 are actually used**                       |
## Rightschifts
a shift right ("_b>>n_") shifts all the bits in _b_ by _n_ to the right
⇒ this is just a division b $2^n$
### logical Rightshift
fills the rest of the bits with 0s
⇒ works only for unsigned division
### arithmetic Rightshift
fills the rest of the bits with whatever the first bit was ⇒ similar to [[Sign Extension]]
⇒ works only for signed division