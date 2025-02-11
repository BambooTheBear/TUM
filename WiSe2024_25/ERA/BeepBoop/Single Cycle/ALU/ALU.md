Die Arithmetic Logic Unit führt alle möglichen (implementierten) Binäre Operationen durch
⇒ Beinhaltet [[Add_Sub]], [[Multiplizierer]], [[Carry Ripple Addierer]]/[[Conditional sum addierer]] und z.B. Bit Operation ([[AND]], [[OR]] etc.)
⇒ Da man immer einen _Takt_ abwarten muss, kann man einfach die Inputs (a, b) durch alle in der ALU verdrahteten Operationen durchpropagieren lassen und dann mit einem [[Multiplexer]] das gewünschte Ergebnis weiterleiten
⇒ "Selector" des Multiplexers kommt aus der [[Control Unit]]