Aus einer "Urne" mit $n$ (unterschiedlichen) Kugeln werden $k$ gezogen
## Ziehen ohne Zurücklegen mit Reihenfolge
⇒ Tupel mit $k$ verschiedenen Einträgen aus $[n]$
$A_{n,k} := \{(s_1, \dots, s_k) \in [n]^k \mid \lvert \{s_1, s_2, \dots, s_k\} \rvert = k\}$
$|A_{n,k}|=\frac{n!}{(n-k)!}$
## Ziehen ohne Zurücklegen ohne Reihenfolge
⇒ $k$-elementige Teilmengen von $[n]$
⇒ $B_{n,k} := \{(s_1, \dots, s_k) \in [n]^k \mid s_1 < s_2 < \dots < s_k\}$
$\lvert B_{n,k} \rvert = \frac{n!}{(n-k)! \, k!}=\binom{n}{k}$ ⇒ [[Binomialkoeffizient]]
## Ziehen mit Zurücklegen mit Reihenfolge
⇒ $k$-elementige Menge mit Elementen aus $[n]$
$\lvert \{(s_1, \dots, s_k) \in [n]^k\} \rvert = n^k.$
## Ziehen mit Zurücklegen ohne Reihenfolge
⇒ Aufsteigend sortierte $k$-Tupel über $[n]$ mit Wiederholungen“
$C_{n,k} := \{(s_1, \dots, s_k) \in [n]^k \mid s_1 \leq s_2 \leq \dots \leq s_k\}$
$\lvert C_{n,k} \rvert = \binom{n+k-1}{k}$
## Zählvektroren
### Summe genau n
⇒ Zählvektoren mit $k$ Einträgen und Summe $n$
$D_{n,k} := \{(s_1, \dots, s_k) \in \mathbb{N}_0^k \mid s_1 + s_2 + \dots + s_k = n\}$
$\lvert D_{n,k} \rvert = \binom{n+k-1}{n}$
### Summe höchstens n
Zählvektoren mit $k$ Einträgen und Summe höchstens $n$
$E_{n,k} := \{(s_1, \dots, s_k) \in \mathbb{N}_0^k \mid s_1 + s_2 + \dots + s_k \leq n\}$
$\lvert E_{n,k} \rvert = \lvert D_{n,k+1} \rvert = \binom{n+k}{n}$
