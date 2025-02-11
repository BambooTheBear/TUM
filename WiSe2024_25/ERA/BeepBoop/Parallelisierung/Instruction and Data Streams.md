# Single Instruction stream | Single Data stream ⇒ SISD
Klassisiches Prozessor Konzept von [[_riscv_single.png|Single Cycle Prozessoren]], jeder _einzelne (single) Instruction Stream_ (Programm) bearbeitet pro Instruktion ein _einzelnes (single) Datum (-Stream)_
# Single Instruction stream | Multiple Data stream ⇒ SIMD
Wenn einzelne Instructions gleichzeitig die Operation auf _multiple Data streams_ anwenden können ⇒ Aus X "Plus-Operationen" auf jeweils ein Datum wird eine "Mega-Plus-Operation" auf X Daten
z.B. Ein Bild mit $1024^2$ Pixeln schwarz weiß färben ⇒ "Multiplikation" auf jeden einzelen Pixel dauert lange, Aber eine GPU die das alles gleichzeitig in einer Operation machen kann ist schneller (sehr spezifische Befehle)
# Multiple Instruction stream | Single Data stream ⇒ MISD
⇒ ??? keine konkrete etablierte umsetzung
# Multiple Instruction stream | Multiple Data stream ⇒ MIMD
klassisches Multithreading ⇒ Mehrere "Hardwarethreads" arbeiten mitseperaten [[ProgrammCounter]], [[Instruktionsspeicher]] und [[Registerbank]], sonst (fast) alles geteilt