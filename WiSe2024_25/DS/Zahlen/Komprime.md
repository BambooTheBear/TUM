$a$ und $b$ sind teilerfremd (koprim) wenn $\text{ggT}(a, b) = 1$
⇒ Die _Komprime_ $\mathbb{Z}_n^*$ von $n$ sind alle Zahlen von $0$ bis $n-1$ die _teilerfremd_ zu $n$ sind
$\mathbb{Z}_n^* := \{k \in \mathbb{Z}_n \mid \text{ggT}(k, n) = 1\}= \mathbb{Z}_n \setminus \bigcup_{p \in \mathbb{P} : p \mid n} \frac{p\mathbb{Z}_n}{p}$
## Eulersche phi Funktion
gibt an wieviele Komprime eine Zahl hat
$\varphi(n) = |\mathbb{Z}_n^*| = n \prod_{p \in \mathbb{P} : p \mid n} \left(1 - p^{-1}\right)$
$\varphi(mn) = \varphi(m)\varphi(n) \quad$ falls $\quad \text{ggT}(m, n) = 1$

$\varphi(p\in\mathbb{P})=p-1$
$\varphi((p\in\mathbb{P})^{r\in \mathbb{R}})=p^{r-1}\cdot(p-1)$
