(all 32bit / 4 Byte)

| ABI   | Register | Description                                 | Saver  |
| ----- | -------- | ------------------------------------------- | ------ |
| zero  | x0       | Always 0                                    | -      |
| ra    | x1       | Return address                              | Caller |
| sp    | x2       | Stack Pointer => use like "0(sp), 4(sp)..." | Callee |
| gp    | x3       | Global Pointer                              | -      |
| tp    | x4       | Thread pointer                              | -      |
| t0-2  | x5-7     | Temporary registers                         | Caller |
| s0/fp | x8       | Saved Register 0 / (Frame Pointer?)         | Callee |
| s1    | x9       | Save Register 1                             | Callee |
| a0-1  | x10-11   | Function Arguments & Return Values          | Caller |
| a2-7  | x12-17   | additional Function arguments               | Caller |
| s2-11 | x18-27   | Saved Register                              | Callee |
| t3-6  | x28-31   | Temporary registers                         | Caller |
 ### Call Save:
- **Caller saved** (= Saver: Caller) ⇒ Caller has to _save_ the registers, because they might change
	→ eg. The caller has to _save_ the _temporary_ register because he cannot expect "temporary" registers to be save from change
 - **Callee saved** (= Saver: Callee) ⇒ Callee cannot change these, or has to make sure they are the same after the called function is done
	 → eg. The callee cant touch _saved registers_ because they are supposed to "safe" from any random sub-programm changes