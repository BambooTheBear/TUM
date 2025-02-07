## Lemma von Bezout
Es gilt für alle $a, b, \alpha, \beta \in \mathbb{Z}$
$\text{ggT}(a, b) = \alpha \cdot a + \beta \cdot b$

## EEA
Der erweiterte Euklidische Algorithmus berechnet für zwei beliebige Zahlen $a \leq b \in \mathbb{Z}$ dir Linearkombination ihres [[Teilbarkeit#ggT|größten gemeinsamen Teilers]] $\text{ggT}(a, b) = \alpha \cdot a + \beta \cdot b$
Der Algorithmus startet mit der folgenden Tabelle und nur $a_1, b_1$ eingefüllt, 
	füllt dann erst $k_1$ und dann
	solange _bis_ $a_{n+1} =0$
		$a_{n+1}, b_{n+1}, k_{n+1}$ aus
	dannach wird $\alpha_n=0, \beta_n=1$ gesetzt und "nach oben" gefüllt 

| n   | $a_n = b_{n-1} \mod a_{n-1}$ | $b_n = a_{n-1}$ | $k_n = \lfloor \frac{b_n}{a_n} \rfloor$ | $\alpha_n = \alpha_{n+1} \alpha_{n+1} + \alpha_{n+1} k_n$ | $\beta_n = \alpha_{n+1}$ |
| --- | ---------------------------- | --------------- | --------------------------------------- | --------------------------------------------------------- | ------------------------ |
| 1   | $7387$                       | $8633$          | $\lfloor 8633 / 7387 \rfloor = 1$       | $1 - 1 \cdot 6 = -7$                                      | $6$                      |
| 2   | $1246$                       | $7387$          | $\lfloor 7387 / 1246 \rfloor = 5$       | $1 - (-1) \cdot 5 = 6$                                    | $-1$                     |
| 3   | $1157$                       | $1246$          | $\lfloor 1246 / 1157 \rfloor = 1$       | $0 - 1 \cdot 1 = -1$                                      | $1$                      |
| 4   | $89$                         | $1157$          | $\lfloor 1157 / 89 \rfloor = 13$        | $1 - 0\cdot13 = 1$                                        | $0$                      |
| 5   | $0$                          | $89$            | $-$                                     | $0$                                                       | $1$                      |
⇒ In jeder Zeile gilt $\text{ggT}(a_{n+1}, b_{n+1}) = \text{ggT}(a_n, b_n) = \alpha_n \cdot a_n + \beta_n \cdot b_n$ 

## Folgerungen aus Bezout/EEA
$\text{ggT}(a, n) = \text{ggT}(b, n) = 1 \quad \iff \quad \text{ggT}(ab, n) = 1;$

$\text{ggT}(a, n) = 1 \qquad\Rightarrow\qquad \text{ggT}(a^k, n) = 1$ für alle $k \in \mathbb{N}_0$.

$n \mid ab$ und $\text{ggT}(a, n) = 1 \qquad\Rightarrow\qquad n \mid b$

$1 = \operatorname{ggT}(a, n) = a\alpha + n\beta \qquad \Rightarrow\qquad a\alpha \equiv_n 1$ und $ax + b \equiv_n 0 \iff x \equiv_n -\alpha b$
#### Lemma von Euklid:
$\operatorname{ggT}(p, ab) = 1 \iff \operatorname{ggT}(p, a) = \operatorname{ggT}(p, b) = 1$
#### Kleiner Fermatscher Satz
Für alle $p\in\mathbb{P}, a\in\mathbb{Z}$ wo $a\notin p\mathbb{Z}$:
$a^{p-1} \equiv_p 1$
#### Eulers Theorem
$\operatorname{ggT}(a, n) = 1 \qquad\Rightarrow \qquad a^{\varphi(n)} \equiv_n 1 \Rightarrow a \cdot a^{\varphi(n)-1} \equiv_n 1.$
