Ein _Matching_ $M$ auf einen [[Graphen#Eigenschaften|bipartiten]] [[Graphen]] $G=(A\uplus B,E)$ (mit $|A|\leq|B|$) ist eine Menge an Kanten $M\subseteq E$ die jedes $a\in A$ mit (höchstens) **einem** $b\in B$ verbindet
(⇒ Ein _perfektes_ Matching weißt jedem $a$ _genau_ ein $b$ zu und vice versa (mit $|A|=|B|$))

### Heiratssatz:
Für jeden $G=(A\uplus B,E)$ gibt es ein Matching $M$ mit $|M|=|A|$ [[gdw. (XNOR)|gdw.]] jede Knotenteilmenge $X \subseteq A$ mindestens $\lvert X \rvert$ Nachbarn (in $B$) besitzt, d.h. falls 
$\lvert \Gamma(X) \rvert \geq \lvert X \rvert$, wobei $\Gamma(X) = \bigcup \Gamma(x)$

## Präferenzmatching
Gesucht ist ein Matching als [[Funktionen von Mengen#bijektiv|bijektive Abbildung]] $f$ von $A$ nach $B$ wobei:
- jedes $a \in A$ hat eine totale Präferenzordnung $\prec_a \subseteq B \times B$; und jedes $b \in B$ entsprechend $\prec_b \subseteq A \times A$
	⇒ z.B. $a_1$: (lieber $b_2$ als $b_1$, aber lieber $b_1$ als $b_4$, aber lieber $b_4$ als $b_3$)

- wichtige Bedingung: $f$ muss stabil sein
	⇒ Falls es KEIN "Paar" $a, a'$ gibt, wo $f(a) \prec_a f(a')$ UND $a' \prec_{f(a')} a$
	 ⇒  $a$ das match von $a'$ preäferiert UND vice versa
### Deferred Acceptance Algorithmus
Mit dem _Gale-Shapley deferred acceptance Algorithmus_ kann für alle $A,B$ eine _stabile_ Abbildung $f$ gefunden werden _in höchstens $O(n²)$ Versuchen_
Für Jedes $b_i\in B, \notin im(f)$:
	$b_i$ geht der Reihe seiner Präferenzen $\prec_{b_i}$ nach alle $a$ durch, die noch nicht "abgelehnt haben"
		Wenn $a$ noch kein "temporäres match" ⇒ $(a, b_i)$ sind temporäres match ⇒ $(a,b_i) \in f$
		Sonst:
			Wenn $b_i\prec_a$"temporäres match von $a$" ($a$ bevorzugt $b_i$) ⇒ neues temporäres match, altes match wieder $\notin im(f)$
			Sonst: $b_i$ zum nächsten $a$ in Präferenzreihe

Anmerkung: keine Garantie eines perfekten Matchings bei nicht-bipartiten-Graphen!