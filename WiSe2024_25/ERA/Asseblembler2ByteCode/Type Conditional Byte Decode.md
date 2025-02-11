Alle (32-Bit) Instruktionen in RISCV haben einen Funktionstyp, der über den OP-Code angegeben ist, je nach Funktionstyp machen die dekodierten Bits etwas anderes:
z.B. ein lui rd, 0xFFFF braucht die 7 OP-Code Bits, 5-Register Bits (da 32 Register, z.B. ist x0 = 00000, a0 = x10 = 01010) und die restlichen 32-7-5=20 Bits können alle für den Upper Immidiate verwendet werden
Vs. z.B. ein addi rd, rs1, 0xFF braucht 2\*5 Register Bits und noch zusätliche Bits zum unterscheiden von addi vs xori 3 funct3 bits ⇒ 7 + 5 + 5 + 3 = 20 bits ⇒ Immidiate höchstens 32-20=12 Bits

![[Pasted image 20250211172610.png]]
