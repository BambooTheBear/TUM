# Datenabhängigkeiten
⇒ Read-After-Write, Write-After-Read, Write-After-Write
⇒ Jede Datenabhängigkeit muss beim "neusortieren" von Befehlen in der Reihenfolge beachtet werden
⇒ z.B. darf   ``addi a0, t0, 1; addi a0, t2, 2``  wegen der Write-After-Write Abhängikeit auf ``a0`` die Reihenfolge nicht umgedreht werden
# Pipeline konflikte
## Datenkonflikte
Datenkonflikte entstehen bei Read-After-Write Abhängigkeiten wenn der Write-Befehl noch nicht die ``Writeback Pahse`` abgeschlossen hat, der Read-Befehl aber schon in ``Execute`` ist.
⇒ Datenkonflikte vermeiden indem mind. **3** Befehle zwischen RAW-Abhängigkeiten bestehen 
⇒ Wenn die [[Registerbank]] des Prozessors in der ersten hälfte des Takts schrieben kann und in der zweiten ließt (statt steigende flanke schreiben, fallende flanke lesen), dann nur **2**!

⇒ z.B. durch NOPs (Not an Operation) ⇒ _Stalling_
⇒ Befehlsumordnung ⇒ Datenabhängigkeiten und Semantik beachten!
⇒ Forwarding ⇒ Das Ergebnis aus dem Write Befehl aus der [[ALU]] direkt in den nächsten Read Befehl forwarden ⇒ fancy _Hazard Unit magic_
## Steuerkonflikte (Control Hazards)
Bei [[Branch]] und [[JUMP]] kann es passieren, dass zu Befehlen gesprungen wird und damit Befehle die eigentlich schon in den ersten Pipelinestufen sind übersprungen werden hätten sollen
⇒ mind. **2** Befehle (NOPs ⇒ Stalling) nach allen potentiellen Control Hazards (jumps/Branches)

⇒ oder Branch Prediction ⇒ "vermutlich überspringen wir die Befehle (oder nicht)" also können wir sie schonmal reinziehen und wenn unsere Vermutung falsch war, alle pipelines _flushen_
⇒ Branch Predition entweder statisch (hardcoded in die hardware) oder dynamisch (on the fly analysieren)
