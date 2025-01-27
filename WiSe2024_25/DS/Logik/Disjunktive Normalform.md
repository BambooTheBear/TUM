Eine [[Aussagenlogische Formeln|boolsche Formel]] ist in der Disjunktiven Normalform (**DNF**) falls alle [[Literale]] in dieser Form sind:
$\bigvee_{i=1}^m \left( \bigwedge_{j=1}^{m_i} L_{i,j} \right)$ ⇒ _[[OR|Disjunktion]]_ an [[AND|Konjunktionen]]
⇒ z.B. $(p \land \neg q) \lor (\neg p \land \neg q \land r) \lor q$

>[!info]
>Eine DNF-Formel ist erfüllbar gdw. mindestens ein Disjunkt erfüllbar ist

## Bildung der Kanonischen DNF
⇒ Kanonisch = für alle aussagenlogisch äquivalenten Formeln _identisch_
Brute-Force indem jede Variable jeder Zeile der Wahrheitstabelle (die zur 1 wird) ver-[[AND|UNDet]] wird und dann ver-[[OR|ODERt]] wird.

Jede [[Aussagenlogische Formeln|Aussagenlogische Formel]] $F$ lässt sich in DNF darstellen:
1. Stelle Wahrheitstabelle zu $F$ auf
2. Bestimme alle minimalen erfüllenden Belegungen von $F$
3. Für jede minimale erfüllende [[Belegung]] $\beta$, bilde die [[AND|Konjunktion]] aller [[Literale]] $p$ aus $F$, bzw. $\lnot p$ wenn $\beta (p) = 0$
	⇒ Minterm
4. Bilde die [[OR|Disjunktion]] aller Minterme 
