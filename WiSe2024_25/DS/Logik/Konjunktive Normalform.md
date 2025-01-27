Eine [[Aussagenlogische Formeln|boolsche Formel]] ist in der Konjunktiven Normalform (**KNF**) falls alle [[Literale]] in dieser Form sind:
$\bigwedge_{i=1}^m \left( \bigvee_{j=1}^{m_i} L_{i,j} \right)$ ⇒ _[[AND|Konjunktion]]_ an [[OR|Disjunktionen]]
⇒ z.B. $(p \lor \neg q) \land (\neg p \lor \neg q \lor r) \land q$

>[!info]
>Eine KNF-Formel ist gültig gdw. alle Konjunkte gültig sind
## Bildung der Kanonischen KNF
⇒ Kanonisch = für alle aussagenlogisch äquivalenten Formeln _identisch_
Brute-Force indem jede Variable jeder Zeile der Wahrheitstabelle (die zur 0 wird) ver-[[OR|ODERt]] wird und dann ver-[[AND|UNDet]] wird.

Jede [[Aussagenlogische Formeln|Aussagenlogische Formel]] $F$ lässt sich in DNF darstellen:
1. Stelle Wahrheitstabelle zu $F$ auf
2. Bestimme alle minimalen _nicht_-erfüllenden Belegungen von $F$
3. Für jede minimale _nicht_ erfüllende [[Belegung]] $\beta$, bilde die [[OR|Disjuktion]] aller [[Literale]] $p$ wenn  $\beta (p) = 0$ aus $F$, bzw. $\lnot p$ wenn $\beta (p) = 1$
	⇒ Minterm
4. Bilde die [[AND|Konjunktion]] aller Minterme 
