Der Davis-Putnam-Logemann-Loveland Algorithmus  ist ein semi-effizienter Algorithmus zu Lösung des [[Erfüllbarkeitsproblem SAT]] von [[Aussagenlogische Formeln]] in der [[Konjunktive Normalform]].

## Algorithmus
### Prequel
Die KNF besteht aus einer [[Mengen|Menge]] [[AND|konjuktivierten]] _Klauseln_ (die leeren Menge an Klauseln $\{\}$ stellt ``true`` da)
Jede _Klausel_ ist eine Menge an [[OR|disjunktiven]] [[Literale|Literalen]] (die leere Klauselmenge $\{\}$ stellt ``false`` da)
⇒ z.B. Die Klauselmenge $\{\{\neg p\}, \{p, \neg q, r\}\}$ stellt die Formel $\neg p \land (p \lor \neg q \lor r)$ da
	⇒ $K=\{\{\},\{p,q\}\}$ wird zu ``false`` da "``false`` $\land x =$ ``false``"
	⇒ $K=\{\}$ wird zu ``true``
### Regeln
Vor jedem Schritt, führe aus bis nicht mehr Möglich
#### 1. OLR
Wenn ein Literal alleine in einer Klausel steht $\{l_i\} \in K$ dann setze $l_i$ zwangsweise auf ``true`` in allen Instanzen von $l_i$
#### 2. PLR
Wenn ein Literal in allen Klauseln nur als $l_i$ bzw $\lnot l_i$ vorkommt, dann setze $l_i$ zwangsweise auf ``true`` in allen Instanzen von $l_i$
#### Wenn $K=\{\}$ 
Wenn $K=\{\}$ dann ist die Formel _erfüllbar_ für die bisher erstellte Belegung
#### OR true
Wenn eine Klausel ein ``true`` enthällt dann Lösche die Klausel
#### OR false
Wenn eine Klausel ein ``false`` enthällt dann Lösche das ``false`` ⇒ kann zu leeren Klauseln führen, NICHT LÖSCHEN sondern beibehalten
### Algorithmus
1. Wähle eine beliebige Variabel $x$
2. Fixiere $x$ auf ``true`` 
	a) ⇒ Wenn nach Anwendung der "OR-true-Regel" $K=\{\}$ ⇒ erfüllbar, beende Algorithmus
	b) ⇒ Wenn nach Anwendung der "OR-false-Regel" $\{\}  \in K$ ⇒ unerfüllbar für diese Belegung, gehe zu 3.
	c) ⇒ Sonst Gehe zu Schritt 1.
3. Fixiere $x$ auf ``false``
	a) ⇒ Wenn nach Anwendung der "OR-true-Regel" $K=\{\}$ ⇒ erfüllbar, beende Algorithmus
	b) ⇒ Wenn nach Anwendung der "OR-false-Regel" $\{\}  \in K$ ⇒ unerfüllbar für diese Belegung, gehe zu 3. für _vorheriges_ $x$
	c) ⇒ Sonst gehe zu Schritt 1.
4. Wenn keine Variablen mehr frei, ⇒ $F$ ist **unerfüllbar**
