Aus einem _Alphabet_ $\Sigma$ (z.B. = $\{a,b,...z\}$) kann man [[Tupel]] = _Wörter_ $w = (a1,\ldots,a_k)\in \Sigma^k$ bilden,
wobei $\Sigma^k$ die Menge aller Wörter der Länge k ist. 
$\Sigma^*$ ist die Menge aller endlichen Wörter aus $\Sigma$

$\Sigma^k := \begin{cases} \{a_1 \dots a_k \mid a_i \in \Sigma \text{ für alle } i \in [k]\} & \text{für } k \geq 1 \\ \{\varepsilon\} & \text{für } k = 0 \end{cases}$
und 
$\Sigma^* = \bigcup_{k \in \mathbb{N}_0} \Sigma^k$

die Teilmenge $L\subseteq\Sigma^*$ ist die _Sprache_ über $\Sigma$
