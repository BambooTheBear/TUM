Eine logische Formel ist **korrekt/(allgemein)gültig** wenn all ihre Instanzen wahr sind ⇒ _Tautologie_
Eine logische Formel ist **widersprüchlihc/unerfüllbar** wenn all ihre Instanzen falsch sind ⇒ _Widerspruch_
Eine logische Formel ist **erfüllbar** wenn es mind. 1 Instanz gibt die wahr ist

Zwei Formeln sind logisch Äquivalent wenn sie für jede [[Belegung]] $\beta$ gilt: $[F](\beta) = [G](\beta)$, also gdw. $F \leftrightarrow G$
⇒ Alle **unterschiedlichen** _Funktionen_ die äquivalent sind, also die selbe [[Funktionen|Funktion]] erfüllen werden über die **Interpretationsfunktion** $\psi$ ihrer Funktion zugewiesen
⇒ "für jede [[Belegung]] $\beta$ gilt: $[F](\beta) = [G](\beta)$" **≙** $F \leftrightarrow G$ **≙** $\psi(F) = \psi(G)$
## Aufstellen von Formeln
- **Wahrheitskonstanten:** `true`, `false`  
- **Unendliche Menge** \( V \) **von Aussagenvariablen:** $p, q, r, s, t, \dots$  
- **Logische Operatoren:** $\neg, \land, \lor, \to$  ([[NOT]], [[AND]], [[OR]]...)
- **Hilfssymbole:** $(, )$

- **Regel 0:** `true` und `false` sind Formeln.  
- **Regel 1:** Eine Aussagenvariable ist eine Formel.  
- **Regel 2:** Ist $F$ eine Formel, dann ist auch $\neg F$ eine Formel.  
- **Regel 3:** Sind $F$ und $G$ Formeln, dann sind  
  $(F \land G)$, $(F \lor G)$ und $(F \to G)$ ebenfalls Formeln.  
- **Regel 4:** Ein Ausdruck ist nur dann eine Formel, wenn er durch Anwendung der oben stehenden Regeln konstruiert werden kann.

## boolsche Algebra
### Bindungsstärke der Operatoren
- $\neg$ bindet stärker als $\land$  
- $\land$ bindet stärker als $\lor$  
- $\lor$ bindet stärker als $\to$
### Rechenregeln

$$
\begin{array}{l l}
(F \land F) \equiv F & \text{(Idempotenz)} \\
(F \lor F) \equiv F & \text{(Idempotenz)} \\[8pt]
(F \land G) \equiv (G \land F) & \text{(Kommutativität)} \\
(F \lor G) \equiv (G \lor F) & \text{(Kommutativität)} \\[8pt]
((F \land G) \land H) \equiv (F \land (G \land H)) & \text{(Assoziativität)} \\
((F \lor G) \lor H) \equiv (F \lor (G \lor H)) & \text{(Assoziativität)} \\[8pt]
(F \land (F \lor G)) \equiv F & \text{(Absorption)} \\
(F \lor (F \land G)) \equiv F & \text{(Absorption)} \\[8pt]
(F \land (G \lor H)) \equiv ((F \land G) \lor (F \land H)) & \text{(Distributivität)} \\
(F \lor (G \land H)) \equiv ((F \lor G) \land (F \lor H)) & \text{(Distributivität)} \\ \\
\neg \neg F \equiv F & \text{(Doppelnegation)} \\ \neg (F \land G) \equiv (\neg F \lor \neg G) & \text{(deMorgan)} \\ \neg (F \lor G) \equiv (\neg F \land \neg G) & \text{(deMorgan)} \\[8pt] (F \land \neg F) \equiv \text{false} & \text{(Triviale Kontradiktion)} \\ (F \lor \neg F) \equiv \text{true} & \text{(Triviale Tautologie)} \\[8pt] (F \land \text{false}) \equiv \text{false} & \text{(Dominanz)} \\ (F \lor \text{true}) \equiv \text{true} & \text{(Dominanz)} \\[8pt] (F \land \text{true}) \equiv F & \text{(Identität)} \\ (F \lor \text{false}) \equiv F & \text{(Identität)} \\ \\
(F \to G) \equiv (\neg F \lor G) & \text{(Implikation)} \\[8pt] (F \leftrightarrow G) \equiv ((F \to G) \land (G \to F)) & \text{(Bikonditional)} \\ (F \leftrightarrow G) \equiv \neg (F \oplus G) & \text{(Bikonditional)} \\[8pt] (F \oplus G) \equiv ((F \lor G) \land (\neg F \lor \neg G)) & \text{(XOR)} \\ (F \oplus G) \equiv ((F \land \neg G) \lor (\neg F \land G)) & \text{(XOR)} \\
\end{array}$$

