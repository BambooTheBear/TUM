Eine _Adjazenz[[Matrix]]_ $A$ auf einen [[Graphen]] $G$:
$A_G = (a_{i,j})_{i,j \in [n]} \in \{0,1\}^{n \times n} \text{ mit } a_{i,j} = 1 \text{ gdw. } v_i E v_j$
⇒ 1 wenn es eine Kante von "Zeile-Knoten" zu "Spalte-Knoten" gibt

Für $k \in \mathbb{N}$ ist $(A_G^k)_{i,j}$ die Anzahl der verschiedenen $k$-Schritt-[[Pfad]]e von $v_i$ nach $v_j$
⇒ Wenn man eine Adjazenzmatrix $k$-mal mit sich selbst multipliziert
### Übergangsmatrix
die Übergangsmatrix $P_G$ eines Graphen $G$ ist eine Adjazenzmatrix aber statt "1" immer $p_{i,j} =\frac{1}{|v_iE|}$
⇒ die Wahrscheinlichkeit dass man von $v_i$ zufällig zu $v_j$ gehen würde
⇒ $(P_G^k)_{i,j}$ ist die Wahrscheinlichkeit von $v_i$ nach $v_j$ in genau $k$ Schritten zu kommen

⇒ Random-Surfer-Modell: Wieviel "Zeit" verbringt ein _random Surfer_ (beginnend bei $v_i$) auf $v_j$
$Q := \left(\frac{1}{T} \sum_{k=0}^{T-1} P_G^k \right)_{i,j}$
