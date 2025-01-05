Ein Baum ist ein _einfacher, zusammenhängender, kreisfreier_ [[Graphen|Graph]]
Jeder Knoten mit $\text{deg}(v)=1$ wird als _Blatt_ bezeichnet, alle anderen als _innere Knoten_

$|E|=|V|-1$
$|V|\geq2 \Rightarrow \text{mind. 2 Blätter}$

"$G$ ist ein Baum" [[gdw. (XNOR)|gdw]]. "$G$ zusammenhängend"$\land |E|=|V|-1$ [[gdw. (XNOR)|gdw]] "$G$ ist kreisfrei"$\land |E|=|V|-1$ [[gdw. (XNOR)|gdw]] "Zwei beliebige Knoten durch genau einen [[Pfad]] verbunden"
## Spannbäume
Ein Spannbaum $T=(V,E')$ ist ein _Teilgraph_ eines [[Graphen]] $G=(V,E)$ mit der selben Knotenmenge $V$ und $E'\subseteq E$
⇒ Jeder Graph hat mind. einen Spannbaum ⇒ Algorithmus z.B. _BFS/DFS_
## Wurzelbäume
Ein Wurzelbaum $G=(V,E,r)$ ist ein Baum $G=(V,E)$ mit einer fest gewählten Wurzel $r\in V$
⇒ Die Höhe $h_G(v)$ eines Knoten v ist der Abstand zur Wurzel
⇒ Die Höge von $G$ ist die längste Entfernung von der Wurzel zu einem Blatt
⇒ Für $u \in V$ ist $(uE^*, E \cap (\frac{uE^*}{2}), u)$ der durch $u$ _induzierte Teilbaum_ von $G$
