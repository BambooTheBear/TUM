Die $k$-_Potenz_ einer [[Gruppe]] ausgehend von einem Elemtent $a$ ist die Operation $k$-mal auf $a$ angewendet
⇒ kann als [[Gruppen als Graphen|Graph]] dargestellt werden

Das _Inverse_ von $a$ ist immer das Element vor dem neutralen Element
Die _Ordnung_ von $a$ = $|\langle a \rangle|$=Ordnung des Inversen von $a$
Es gibt  $\frac{|\mathbb{G}|}{|\langle a \rangle|}$ [[Kreis|Kreise]] in dem [[Graphen]] der [[Permutationen]] der Gruppe ausgehend von a ⇒ [[Gruppen als Graphen]]
$a$ ist ein _Erzeuger_ wenn $|\langle a \rangle|=|\mathbb{G}|$ ⇒ nur ein Kreis
## additiv
Sei $\mathbb{G}$ eine [[Gruppe]]. Für alle $a \in \mathbb{G}$ und $k \in \mathbb{N}_0$:
$ka$ $(-ka)$ bezeichnet die Summe von $k$ Kopien von $a$ $(-a)$.

$\langle a \rangle := \langle \{ a \} \rangle = \{ ka \mid k \in \mathbb{Z} \} = \{ \dots, -3a, -2, -a, 0, a, 2a, 3a, \dots \}$

## multiplikativ
Sei $\mathbb{G}$ eine [[Gruppe]]. Für alle $a \in \mathbb{G}$ und $k \in \mathbb{N}_0$:
$a^k$ $(a^{-k})$ bezeichnet das Produkt von $k$ Kopien von $a$ $(a^{-1})$

Dabei gilt: $a^k = a^{k \mod |\mathbb{G}|} = a^{k \mod \lambda_{\mathbb{G}}} = a^{k \mod \operatorname{ord}(a)}$

$\langle a \rangle := \langle \{ a \} \rangle = \{ a^k \mid k \in \mathbb{Z} \} = \{ \dots, a^{-3}, a^{-2}, a^{-1}, 1, a, a^2, a^3, \dots \}$
### Beispiel $(\mathbb{Z}_{11}^*, \cdot_{11}, 1)$:
$\langle 1 \rangle \quad = \quad \{1\}$  
$\langle 2 \rangle \quad = \quad \{2, 4, 8, 5, 10, 9, 7, 3, 6, 1\}$  
$\langle 3 \rangle \quad = \quad \{3, 9, 5, 4, 1\}$  
$\langle 4 \rangle \quad = \quad \langle 3 \rangle$  
$\langle 5 \rangle \quad = \quad \{5, 3, 4, 9, 1\}$  
$\langle 6 \rangle \quad = \quad \langle 2 \rangle$  
$\langle 7 \rangle \quad = \quad \{7, 5, 2, 3, 10, 4, 6, 9, 8, 1\}$  
$\langle 8 \rangle \quad = \quad \langle 7 \rangle$  
$\langle 9 \rangle \quad = \quad \langle 5 \rangle$  
$\langle 10 \rangle \quad = \quad \{10, 1\}$
