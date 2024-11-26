Eine **Menge** ist eine Ansammlung an Objekten, unabhängig von Reihenfolge, Kardinalität oder Typ der Objekte
⇒ {1,2,1,1,grün,blau,{3,2,{ }}} = {2,grün,{3,2,{ }},blau,1}
## Operationen
- _explizite Menge:_ A={1,2,3}
- _implizite Menge:_ B={2x | x $\in$ A}
- _leere Menge:_ { } = ∅
- $M_1 \subseteq M_2 = \forall (x \in M_1), (x \in M_2) = M_1 \text{ ist Teilmenge von } M_2$
- $M_1 \subset M_2 = \forall (x \in M_1), (x \in M_2) \land M_1 \neq M_2 = M_1 \text{ ist echte Teilmenge von } M_2$
- $M_1 \neq M_2 = \exists (x \in M_1) \lor (x \in M_2), (x \notin M_1 \cup M_2) = M_1 \text{ und } M_2 \text{ sind nicht gleich}$
- $M_1 \supseteq M_2 = \forall (x \in M_2), (x \in M_1) = M_1 \text{ ist Obermenge von } M_2$
- $M_1 \setminus M_2 = \{ x \in M_1 \mid x \notin M_2 \} = M_1 \text{ ohne Elemente aus } M_2$
- $M_1 = M_2 = \forall (x \in M_1), (x \in M_2) \land \forall (x \in M_2), (x \in M_1) = M_1 \text{ und } M_2 \text{ sind gleich}$
- $M_1 \triangle M_2 = M_1 \oplus M_2 = (M_1 \setminus M_2) \cup (M_2 \setminus M_1) = \text{symmetrische Differenz von } M_1 \text{ und } M_2$
- $|M| = \text{Anzahl der Elemente in } M = \text{Kardinalität von } M$
- $M_1 \cap M_2 = \{ x \mid x \in M_1 \land x \in M_2 \} = \text{Schnittmenge von } M_1 \text{ und } M_2$
- $M_1 \cup M_2 = \{ x \mid x \in M_1 \lor x \in M_2 \} = \text{Vereinigung von } M_1 \text{ und } M_2$
- $M_1 \cap M_2 = \emptyset = M_1 \text{ und } M_2 \text{ sind disjunkt}$
- $\Omega = \text{alle Elemente des Universums}$
- $\bar{A} = \{ x \in \Omega \mid x \notin A \} = \text{Komplement von } A \text{ im Universum}$
 
- $\mathcal{P}(M) = \{ S \mid S \subseteq M \}$ = [[Potenzmenge]] von M
- $\cap S = \cap _{M\in S} M= \{ x \mid \text{für jedes M in S gilt x in M} \} = \text{nur die x die in alle Mengen in S sind}$
- $\cup S = \cup _{M\in S} M= \{ x \mid \text{Es gibt mind. 1 M in S mit x in M} \} = \text{alle Elemente in allen Mengen in S}$
### Rechenregeln
- $A \cup B = B \cup A = \text{Vereinigung ist kommutativ}$ 
- $A \cap B = B \cap A = \text{Schnittmenge ist kommutativ}$ 
- $(A \cup B) \cup C = A \cup (B \cup C) = \text{Vereinigung ist assoziativ}$ 
- $(A \cap B) \cap C = A \cap (B \cap C) = \text{Schnittmenge ist assoziativ}$ 

- $A \cup (A \cap B) = A = \text{Absorptionsgesetz für die Vereinigung}$ 
- $A \cap (A \cup B) = A = \text{Absorptionsgesetz für die Schnittmenge}$ 

- $A \cup (B \cap C) = (A \cup B) \cap (A \cup C) = \text{Distributivgesetz der Vereinigung über die Schnittmenge}$ 
- $A \cap (B \cup C) = (A \cap B) \cup (A \cap C) = \text{Distributivgesetz der Schnittmenge über die Vereinigung}$

- $\overline{A \cup B} = \overline{A} \cap \overline{B} = \text{Das Komplement der Vereinigung ist der Schnitt der Komplemente}$
- $\overline{A \cap B} = \overline{A} \cup \overline{B} = \text{Das Komplement des Schnitts ist die Vereinigung der Komplemente}$



## Kartesisches Produkt
Für zwei Mengen A, B ist das _kartesische Produkt_ $A\times B = \{(a,b)|a\in A, b\in B\}$
$A^k = \times\prod_{i=0}^k A = \{ (a_1, a_2, \ldots, a_k) \mid a_1 \in A, a_2 \in A, \ldots a_k \in A\}$
$A^0=\{()\}, A^1 \neq A$
