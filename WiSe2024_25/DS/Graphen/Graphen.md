Ein _gerichteter Graph (Digraph)_ $G=(V,E)$  mit der _Knotenmenge_ V und der [[Binäre Relationen|binären Relation]] (Kantenmenge) $E \subseteq V\times V$ 
_Ein Graph kann auch ungerichtet sein ⇒ kein Digraph_

## Eigenschaften
- G ist _**endlich**_ falls V endlich ist
- G ist _**ungerichtet**_ falls E [[Binäre Relationen#Eigenschaften|symmetrisch]] ist
- G ist _**einfach**_ falls E [[Binäre Relationen#Eigenschaften|symmetrisch]]  und [[Binäre Relationen#Eigenschaften|irreflexiv]] ist ⇒ $\{u, v\} \in E \subseteq \binom{V}{2}$
- G ist _**bipartit**_ falls es [[Mengen]] $A \cup B=V$ gibt sodass es nur Kanten zwischen A und B gibt, aber keine innerhalb dieser Knotenmengen
- G ist _**zusammenhängend**_ falls $u(E \cup E^{-1})^*v$ gilt ⇒ Wenn es einen zwischen allen möglichen Knotenpaaren einen Pfad (unabhängig der Richtung) gibt
- G ist _**stark zusammenhängend**_ falls $uE^*v$ gilt ⇒ Wenn es einen zwischen allen möglichen Knotenpaaren einen Pfad gibt
- $U \subseteq V$ ist eine (starke) Zusammenhangskomponente, falls $G[U]$ (stark) zusammenhängend ist
- $U$ ist eine maximale (starke) Zusammenhangskomponente, falls es kein $U'$ mit $U \subsetneq U' \subseteq V$ gibt, so dass $G[U']$ selbst eine (starke) Zusammenhangskomponente ist
### Lemma
- Ein Einfacher Graph ist _bipartit_ gdw. er _keinen [[Kreis]] ungerader Länge_ enthält
- Jeder _einfache zusammenhängende_ Graph mit n Knoten hat mindestens _n-1 Kanten_
- Jeder endliche einfache Graph mit $n\geq3$ Knoten und mindestens _n Kanten_ hat einen _[[Kreis]]_
## Isomorphie
Zwei Digraphen sind _isomorph_ ($G \cong H$)zu einander wenn es eine [[Funktionen von Mengen#bijektiv|bijektive]] [[Funktionen|Funktion]] $\beta: V_G \rightarrow V_H$ gibt, die die Kanten der jeweiligen Knoten respektiert
![[Pasted image 20241225145307.png]]
### Graphautomorphismus
Ein Graph kann _Automorphismen_ haben, also Isomorphien des Graphen auf sich selber

## Gradfolgen
Jedem (einfachen) Graphen kann man eine _sortierte_ Gradfolge $(deg(v_1),deg(v_2),...,deg(v_n))$ zuweisen
Ein Graph heißt _k-regulär_ wenn alle Knoten den Grad k haben
⇒ "Handschlaglemma" $2 \lvert E \rvert = \sum_{i \in [n]} \deg(v_i)$
⇒ Graph mit $\lvert V \rvert > \frac{1}{2} \sum_{i \in [n]} d_i + 1$ kann nicht zsm. hängend sein
⇒ Man kann anhand von Gradfolgen erkennen ob der Graph realisierbar ist mit dem [[TODO Havel-Hakimi-Algorithmus]]
## spezielle Formen
### Vollständiger Graph $K_n$
$K_n = ([n],\binom{[n]}{2}$
⇒ Graph wo alle Knoten mit allen anderen Knoten verbunden sind
⇒ $|E_{K_n}|=\frac{n(n-1)}{2}$ und $\text{deg}(v)=n-1$
⇒ (n-1)-regulär
⇒ $\chi=n$ ([[Knotenfärbung|chromatische Zahl]])

### Kreisgraph $C_n$
$C_n := ([n], \{\{i, (i \mod n) + 1\} \mid i \in [n]\})$
⇒ 2-regulär
⇒ gerades n → $\chi=2$, ungerades n → $\chi =3$ 
### Pfadgraph $P_n$
$P_n := ([n], \{\{i, i+1\} \mid i \in [n-1]\})$
### vollständiger bipartiter Graph $K_{m,n}$
$K_{m,n} := ([m+n], \{\{i,j\} \mid i \in [m], j \in [m+n] \setminus [m]\}) \quad (m \leq n)$
⇒ ein bipartiter Graph wo jeder Knoten der einen Seite mit allen Knoten der anderen Seite verbunden ist
⇒ $\chi=2$ ([[Knotenfärbung|chromatische Zahl]])
### Gittergraph $M_{m,n}$
$M_{m,n} := ([m] \times [n], \{\{(i,j), (k,l)\} \mid \lvert i-k \rvert + \lvert j-l \rvert = 1\})$
Ein $m\times n$ großes Gitter als Graph
### Hyperwürfel $Q_n$
$Q_n := (\{0,1\}^n, \{\{u,v\} \mid \sum_{i=1}^n \lvert u_i - v_i \rvert = 1\}) \text{ mit } Q_0 := (\{\varepsilon\}, \emptyset)$
⇒ n-regulär
![[Pasted image 20241225193432.png]]
### perfekter Binär[[baum]] $B_h$
Höhe h mit $B_0$ = ein Knoten
$B_h := (\{0,1\}^{\leq h}, \{\{u, ux\} \mid u \in \{0,1\}^{< h}, x \in \{0,1\}\})$
⇒ Insgesamt $2{h+1}-1$ Knoten mit $2^h$ Blättern