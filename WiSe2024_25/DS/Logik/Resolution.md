Die _Resolution_ wird verwendet um eine [[Aussagenlogische Formeln|aussachelogische Formel]] $F$ auf _Unerfüllbarkeit_ zu prüfen, der Algorithmus terminiert immer.
Kann auch verwendet werden zum Beweis der _Allgemeingültigkeit_ mit $F \text{ allgemeingültig} \leftrightarrow \lnot F \text{ unerfüllbar}$ 

Dafür wird die [[Konjunktive Normalform]] von $F$ gebildet und dann für jedes Paar von Klauseln wenn es möglich ist der _Resolvent_ zu $F$ hinzugefügt
⇒ Resolvent ist die transitive [[if _ then _|Implikation]] der beiden Klauseln via $A \rightarrow B = \lnot A \lor B$ und $B \rightarrow C = \lnot B \lor C$, somit $A\rightarrow C =  \lnot A \lor C$
	z.B. Die Klauseln $\{\neg p, q, r\}$, $\{\neg r, s, t\}$, und $\{\neg p, q, s, t\}$ sind äquivalent zu  $(p \land \neg q) \to r \quad r \to (s \lor t) \quad (p \land \neg q) \to (s \lor t)$
⇒ Der Resolvent von $\{p\}$ und $\{\lnot p\}$  ist ``false`` und somit die leere Menge
⇒ Solange über neue Literale zusätsliche "implizierte" Resolventen expliztit hinzufügen, bis ``false`` in $F$ ⇒ unerfüllbar
(⇒ statt ``false`` auch oft die leeren Menge $\{\}$ oder $\square$)

$\text{Res}^0(F) := F$  
$\text{Res}^{k+1}(F) := \text{Res}^k(F) \cup \{(K_1 \setminus \{L\}) \cup (K_2 \setminus \{\overline{L}\}) \mid K_1, K_2 \in \text{Res}^k(F), L \in K_1, \overline{L} \in K_2\}$  
$\text{Res}^*(F) := \bigcup_{k \in \mathbb{N}_0} \text{Res}^k(F)$
![[Pasted image 20250127151220.png]]
