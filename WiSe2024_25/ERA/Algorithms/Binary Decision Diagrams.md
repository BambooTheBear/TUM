BDDs = Darstellung einer boolschen [[Funktionen|Funktion]] als gerichteter azyklischer [[Graphen|Graph]] (DAG)
![[Pasted image 20250212132647.png]]
Konstruktion mittels "Shannon-Zerlegung" ⇒ Setze eine Variabel auf 0, was für eine Formel übrigbleibt ist unterer teilbaum und analog zur 1
## I-Reduktion
Isomorphe Knoten zusammenführen
⇒ Wenn "Teil-Formeln" identisch sind, könenn sie zu einem Knoten zusammengeführt werden
![[Pasted image 20250212132948.png]]
## S-Reduktion
Wenn ein Knoten nur ein "unnötiger" zwischenschritt vor einem anderen Knoten ist (also beide pfade aus a in b gehen) kann er entfernt werden
![[Pasted image 20250212133031.png]]
# Variablenordung
Das finden einer optimalen Variablenordnung ist [[Erfüllbarkeitsproblem SAT|NP-hard]] Problem, aber man kann durch vertauschen von (in der variablen Ordnung) aufeinanderfolgenden Variablen den BDD einfach umformen, ohne ihn neu zu bilden
![[Pasted image 20250212133240.png]]
⇒ möglicherweise neue Reduktionen möglich