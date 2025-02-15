Eine _binäre_ [[Relationen|Relation]] ist eine 2-stellige Relation $R\subseteq A\times B$
Binäre Relationen können als [[Graphen]] visualisiert werden

## Eigenschaften
$R\subseteq A\times A$
- reflexiv ⇒ $R^0 \subseteq R$
	- irreflexiv ⇒ $R^0\cap R=\emptyset$
- symmetrisch ⇒ $\forall (s,t)\in R:(t,s) \in R$
- assymmetrisch ⇒ $\forall (s,t)\in R:(t,s) \notin R$ ( ⇒ immer irreflexiv)
- antisymmetisch ⇒ $(s,t) \in R \land (t,s) \in R ⇒ s=t$
- transitiv ⇒ $\forall (s,t),(t,u)\in R:(s,u) \in R$ 

## Äquivalenzrelationen
Eine binäre Relation $R\subseteq A\times A$ ist eine _Äquivalenzrelation_ bzgl. der [[Mengen|Menge]] A wenn sie _symmetrisch, reflexiv und transitiv_ ist
⇒ z.B. "a=b" oder "a%m=b%m"
⇒ man kann die Objekte der Universums bzgl. der Relation in [[Potenzmenge#Partitionen|Partitionen]] unterteilen:
z.B. "a%3=b%3" → $\{3\mathbb{Z},3\mathbb{Z}+1, 3\mathbb{Z}+2\}$
⇒ die _Äquivalenzklasse_ eines Objekts a bzgl. R ($[a]_R$) ⇒ "in welche Partition es fällt" ⇒ $[-5]_{(\%3)} = 3 \mathbb{Z}+1$

## Ordnungsrelationen
Eine binäre Relation $R\subseteq A\times A$ ist eine _Ordnungsrelation_ bzgl. der [[Mengen|Menge]] A wenn sie _antisymmetrisch, reflexiv und transitiv_ ist
⇒ z.B. "a$\leq$b" oder "X$\subseteq$Y"
⇒ die Relation "ordnet" die Objekte (partiell)
### totale Ordnung
jede Ordnungsrelation ist eine _partielle Ordnung_, wenn zusätzlich noch gilt "jedes Objekt steht in Relation zu jedem anderen Objekt" dann nennt man das _totale Ordnung_
⇒ z.B. "a$\leq$b" oder "X$\subseteq$Y" aber **nicht** "a ist durch b teilbar" da 2 und 3 in keiner Relation stehen

### Begriffe
- $m\in A$ ist ein _maximales_ Element falls es keine Kanten **zu** einem anderen Element hat
- $m\in A$ ist das _größte_ Element falls es maximal ist und alle Elemente zu ihm zeigen
- $m\in A$ ist ein _minimales_ Element falls es keine Kanten **von** einem anderen Element hat
- $m\in A$ ist das _kleinste_ Element falls es minimal ist und auf alle Elemente zeigt
- $R^{-1}$ ist die _inverse Relation_ ⇒ Pfeile umdrehen
