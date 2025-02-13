Die Überprüfung ob 2 Schaltkreise IMMER äquivalent sind (für jede Belegung) lässt sich auf ein [[Erfüllbarkeitsproblem SAT]] zurückführen und das dann mit eine SAT Solver lösen ⇒ Auf Erfüllbarkeit prüfen
Idee: Schaltkreis $A$ und Schaltkreis $B$ sind äquivalent gwd. $A\leftrightarrow B$ immer gilt ⇒ gdw. $\overline{A\leftrightarrow B}$ unerfüllbar ⇒ gdw. $A\oplus B$ unerfüllbar ⇒ gdw. SAT-SOLVER($A\oplus B$) =``UNSAT``
$A\oplus B$ = _Miterschaltkreis_ ⇒ durch [[Tseitin Transformation]] zur [[Konjunktive Normalform]] bilden und dann in SAT-Solver

z.B. sind $\overline{A\land B}$ und $\overline{A}\lor \overline{B}$ äquivalent?
![[Pasted image 20250212134015.png]]