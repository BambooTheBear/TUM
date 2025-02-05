Eine Gruppe $\mathbb{G}$ wird notiert durch $\mathbb{G}$ ≙ $(\mathbb{G}, \text{Operator}, \text{neutrales Element})$
Eine _valide_ **Gruppe** ist abhängig vom _Operator_ additiv oder multiplikativ
### additive Gruppen
Eine Gruppe ist _additiv_ (z.B. $\mathbb{G}$≙$(\mathbb{Z}, +, 0)$) wenn sie:
- abgeschlossen ⇒ $+: \mathbb{G} \times \mathbb{G} \to \mathbb{G}$
- assoziativ ⇒ $(a + b) + c = a + (b + c)$
- kommutativ ⇒ $a+b=b+a$
- das neutrale Element funktioniert ⇒ $a + 0 = 0 + a = a$
- für jedes $a$ ein _Inverses_ existiert ⇒ $a + b = b + a = 0$

⇒ valide additive Gruppen: $(\mathbb{R}, +, 0)$, $(\mathbb{Z}, +, 0)$
### multiplikative Gruppen
Eine Gruppe ist _multiplikativ_ (z.B. $\mathbb{G}$≙$(\mathbb{R}, \cdot, 1)$) wenn sie:
- abgeschlossen ⇒ $\cdot: \mathbb{G} \times \mathbb{G} \to \mathbb{G}$
- assoziativ ⇒ $(a \cdot b) \cdot c = a \cdot (b \cdot c)$
- das neutrale Element funktioniert ⇒ $a \cdot 1 = a$
- für jedes $a$ ein _Inverses_ existiert ⇒ $a \cdot b  = 1$

⇒ eine multiplikative Gruppe kann auch kommutativ ⇒ $a \cdot b = b \cdot a$ sein

⇒ valide multiplikative Gruppen: $(\mathbb{R}, \cdot, 1)$, $(\mathbb{Q}, \cdot, 1)$, $(\mathbb{Z}, \cdot, 1)$

## Eigenschaften
$|\mathbb{G}|$ ist die _Gruppenordung_,
$\mathbb{G}$ ist _endlich_ fallls die Gruppenordung _nicht unendlich_ ist

$H \subseteq \mathbb{G}$ ist eine Untergruppe von $(\mathbb{G}, \cdot, 1)$, wenn $(H, \cdot, 1)$ eine Gruppe ist

Der **Exponent** einer **endlichen** Gruppe $(\mathbb{G}, \cdot, 1)$ ist: $\lambda_{\mathbb{G}} := \operatorname{kgV}(\{\operatorname{ord}(a) \mid a \in \mathbb{G} \}) = \min \{ \lambda \in \mathbb{N} \mid \text{ für alle } a \in \mathbb{G}: a^\lambda = 1 \}$


### isomorph
Zwei Gruppen $(\mathbb{G}_1, \cdot_1, 1_1)$, $(\mathbb{G}_2, \cdot_2, 1_2)$ sind _isomorph_ $(\mathbb{G}_1 \cong \mathbb{G}_2)$, wenn eine [[Funktionen von Mengen#bijektiv|Bijektion]] $h: \mathbb{G}_1 \xrightarrow{\text{bij}} \mathbb{G}_2$ mit $h(a \cdot_1 b) = h(a) \cdot_2 h(b)$ für alle $a, b \in \mathbb{G}_1$ existiert.
⇒ z.B. sind $(\mathbb{Z}_6, +_6, 0)$ und $(\mathbb{Z}_9^*, \cdot_9, 1)$ isomorph mittels $h: \mathbb{Z}_6 \to \mathbb{Z}_9^*, \; x \mapsto (2^x) \mod 9$

### symmetrische Gruppen
$(\mathcal{S}_A, \circ, \operatorname{Id}_A)$ symmetrische Gruppe über $A$:
- Grundmenge: $\mathcal{S}_A = \{ f: A \to A \mid f \text{ bijektiv} \}$
- Gruppenoperation: $f \circ g: A \to A: a \mapsto f(g(a))$ (Funktionskomposition)
- Neutrales: Identität $\operatorname{Id}_A: A \to A: a \mapsto a$
- Inverse: Umkehrabbildung

$\mathcal{S}_n$ kurz für die Menge $\mathcal{S}_{[n]}$ aller [[Permutationen]] von $[n]$.

#### Cayley table
z.B. $(\mathcal{S}_3, \circ, \operatorname{Id})$

|          | $\operatorname{Id}_{[3]}$ | (1,2) | (1,3) | (2,3) | (1,2,3) | (1,3,2) |
|----------|-----------------|-------|-------|-------|---------|---------|
| $\operatorname{Id}_{[3]}$ | $\operatorname{Id}_{[3]}$ | (1,2) | (1,3) | (2,3) | (1,2,3) | (1,3,2) |
| (1,2)   | (1,2) | $\operatorname{Id}_{[3]}$ | (1,3,2) | (1,2,3) | (2,3) | (1,3) |
| (1,3)   | (1,3) | (1,2,3) | $\operatorname{Id}_{[3]}$ | (1,3,2) | (1,2) | (2,3) |
| (2,3)   | (2,3) | (1,3,2) | (1,2,3) | $\operatorname{Id}_{[3]}$ | (1,3) | (1,2) |
| (1,2,3) | (1,2,3) | (1,3) | (2,3) | (1,2) | (1,3,2) | $\operatorname{Id}_{[3]}$ |
| (1,3,2) | (1,3,2) | (2,3) | (1,2) | (1,3) | $\operatorname{Id}_{[3]}$ | (1,2,3) |
