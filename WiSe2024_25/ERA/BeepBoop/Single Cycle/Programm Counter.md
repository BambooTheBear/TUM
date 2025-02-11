Der Programm Counter hat immer die Addresse des nächsten Befehls
⇒ Mit der Clock verbunden um jeden Taktzyklus einen neuen PC auszugeben
![[Pasted image 20250211173129.png]]
wird standardmäßig um 4 Erhöht (4 Byte = 32 Bit Architektur) kann aber auch anders gesetzt werden über [[JUMP]] oder [[Branch]]
⇒ Verbunden mit "+4" Addierer und dem Ergebnis der [[ALU]] und dann einem [[Multiplexer]] der enscheidet ob es ein JUMP/Branchbefehl ist (basierend auf der [[Control Unit]])