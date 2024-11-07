the Stack (Kellerspeicher) can be used to store an "infinite" amount of data without worrying about limited amount of registers, constant addresses, overwriting other functions, etc.
the stack "grows" from top to bottom, so the most recent item is at the lowest address in the stack.
the [[Convention]] uses the "sp"-[[Register]] to store the _**Stackpointer**_ (the "top" of the Stack)
the sp in RiscV addresses Bytes, to store a 32-bit register value, you need to allocate 4 stackspaces, the execution takes care of [[LittleEndian]]
### Push
```
addi sp, sp, -4 //decrement stackpointer by 4 ⇒ "above" the sp there is now space for 4 byte
sw rs, 0(sp) //write the contents(word) from the rs into the address the Stackpointer is directing to
```
### Pop
```
lw rd, 0(sp) //write the word from the top of the stack (Stackpointer) into rd
addi sp, sp, 4 //increment stackpointer so that the new "top" is at the next word of the stack
```
