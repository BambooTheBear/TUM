$F$ ist erfüllbarkeitsäquivalent zu $G$ ($F \equiv_e G$) gdw. Für die beiden [[Aussagenlogische Formeln]] gilt: "$F$ ist **erfüllbar** gdw. $G$ erfüllbar ist"
⇒ Bei zwei erfüllbarkeitsäquivalenten Formeln müssen die _erfüllenden_ [[Belegung|Belegungen]] $\beta_F$ und $\beta_G$ nicht zur jeweils anderen Formel passen
	⇒ z.B. $A \lor B \equiv_e C \land (C \leftrightarrow (A \lor B)) \text{ aber } A \lor B \not\equiv C \land (C \leftrightarrow (A \lor B))$

## Konstruktion einer zu $F$ erfüllbarkeitsäquivalenten Formel in [[Konjunktive Normalform|KNF]]
### Ansatz: 
Man erstellt für jeden Teilbaum eine neue "Hilfsvariabel" $p_i$, dadurch ist jeder Teilbaum definierbar durch $p_i$≙"$p_j x p_k$"            mit $x \in$ (einer der [[Operatoren]])
Dann gilt ja $p_i \leftrightarrow (p_jxp_k)$, man fügt also $p_i \leftrightarrow (p_jxp_k)$ zu $E_F$ hinzu.

### Algorithmus
⇒ [[Tseitin Transformation]]?
Man nehme eine belibige [[Aussagenlogische Formeln|Boolsche Formel]] $F$ mit beliebigen **binären** [[Operatoren]] und Konstruiere den [[Syntaxbaum]]
Sei $E_F$ die zu bildende Formeln mit $E_F \equiv_e F$

Starte mit $E_F = p_0$
Für jeden Teilbaum $p_i$ (auch dem Wurzelknoten):
	1. Wenn $p_i=q_j$ mit $q_j$ als elementare Variabel ⇒  dann füge $(p_i \leftrightarrow q_j)$ zu $E_F$ hinzu ⇒  $E_F = (p_i \leftrightarrow q_j) \land E_F$
	2. Wenn $p_i = \lnot p_j$ mit $p_j$ als weiterer Teilbaum ⇒ dann füge ($p_i \leftrightarrow \lnot p_j$) zu $E_F$ hinzu ⇒ $E_F = (p_i \leftrightarrow \lnot p_j) \land E_F$
	3. Wenn $p_i=p_j x p_k$ mit $x \in$ (einer der [[Operatoren]]) ⇒ dann füge $p_i \leftrightarrow (p_jxp_k)$ zu $E_F$ hinzu ⇒ $E_F = (p_i \leftrightarrow (p_jxp_k)) \land E_F$

⇒ Resultierende $E_F$ ist erfüllbarkeitsäquivalent zu $F$ und _einfach_ in die [[Konjunktive Normalform|KNF]] umformbar
⇒ $E_F$ ist "kleiner" als die [[Konjunktive Normalform#Bildung der Kanonischen KNF|Kanonische KNF]] aber *erfüllbarkeitsäquivalent* und eine $E_F$ erfüllende Belegung $\beta$ erfüllt auch immer $F$
⇒ Folglich kann die "kleine" $E_F$ in einem [[Erfüllbarkeitsproblem SAT|SAT Solver]] effizient gelöst und eine erfüllende Belegung $\beta$ für $F$ gefunden werden