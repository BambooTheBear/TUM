**Def.:** Eine **Belegung** ist eine [[Funktionen|Funktion]] $\beta : V' \to \{0, 1\}$ mit $V' \subseteq V$.  
Die Belegung $\beta : V' \to \{0, 1\}$ _passt_ zu einer [[Aussagenlogische Formeln|Aussagelogischen Formeln]] $F$, falls $V_F \subseteq V'$ (jede in $F$ vorkommende Variable ist in $V'$ enthalten).
Eine zu $F$ passende Belegung $\beta : V' \to \{0, 1\}$ heißt _**minimal**_, falls $V_F = V'$ ($V'$ ist die Menge aller in $F$ vorkommenden Variablen).

**Wahrheitswert** $[F](\beta)$ von $F$ unter $\beta$:
$$[F](\beta) := \begin{cases} 1 & \text{falls } F = \text{true}, \\ 0 & \text{falls } F = \text{false}, \\ \beta(p) & \text{falls } F = p \text{ für } p \in V, \\ 1 - [G](\beta) & \text{falls } F = \neg G, \\ \max\{[G](\beta), [H](\beta)\} & \text{falls } F = (G \lor H), \\ \min\{[G](\beta), [H](\beta)\} & \text{falls } F = (G \land H), \\ \max\{1 - [G](\beta), [H](\beta)\} & \text{falls } F = (G \to H). \end{cases}$$
