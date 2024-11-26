$\text{Sind } R \subseteq A \times B \text{ sowie } S \subseteq C \times D \text{ binäre Relationen, dann ist das relationale Produkt von } R \text{ und } S \text{ die binäre Relation } RS \subseteq A \times D \text{ gegeben durch}$
$RS = \{(a, d) \mid \text{es gibt } x \in B \cap C \text{ mit } (a, x) \in R \text{ und } (x, d) \in S\}$
⇒ RS ist die _Verkettung_ von R und S

## rel. Produkt bin. Relation
eine [[Binäre Relationen|binäre Relation]] kann mit sich selbst verkettet werden wenn $R\subseteq A \times A$
$R^0 := \text{Id}_A := \{(a, a) \mid a \in A\}$
$R^1 := R = R^0 R$
$R^2 := RR = R^1 R$
$R^{k+1} := R^k R = RR^k = \underbrace{RR \dots R}_{k+1 \text{ mal}} \text{ für beliebiges } k \in \mathbb{N}_0.$
⇒ $R^k$ ist der Graph aller [[Pfad|Pfade]] der Länge k im ursprünglichen [[Graphen]] von $R$
### transitive Hülle
die _transitive Hülle_ einer [[Binäre Relationen|binären Relation]] ist die Menge aller Pfade die in endlichen Schritten _transitiv_ erreichbar waren
⇒ $R^+ := \bigcup_{k \in \mathbb{N}} R^k$
#### reflexiv transitive Hülle
dir _reflexiv transitive Hülle_ ist das gleiche wie die transitive Hülle, aber jeder Knoten hat noch eine Relation zu sich selber.
⇒ $R^* := \bigcup_{k \in \mathbb{N}_0} R^k = R^0 \cup R^+$
⇒ v ist von u "erreichbar" wenn $(u,v)\in R^* = u R^* v$

