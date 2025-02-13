Ein [[_riscv_single.png|Single Cycle Prozessor]] kann effizienter gemacht werden indem er in 5 Unterstufen aufgeteilt wird ⇒ Fetch, Decode, Execute, Writeback und dann alle Befehle die hinteinander folgen direkt in die Phase davor einsteigen können, statt auf die volle Beeningung des Vorgängers zu warten.
⇒ Dafür einfach zwischen die 5 Phasen [[D-Latch|Flip Flops]] einfügen die die Voregrbenisse alle gleichzeitig durch propagieren
⇒ Speedup von max. Anzahl der Pipeline Stufen (bei uns immer 5, kann aber auch unterschiedlich sein)
⇒ Speedup Formel: $\frac{\text{Laufzeit mit Pipeline}}{\text{Laufzeit ohne Pipeline}}$
![[Pasted image 20250212003337.png]]

