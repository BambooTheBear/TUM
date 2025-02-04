$n$ teilt $m$ ganzzahlig:                                                          $n \mid m \iff \frac{m}{n} \in \mathbb{Z} \iff m \in n\mathbb{Z} := \{kn \mid k \in \mathbb{Z}\}$
kleinstes gemeinsames Vielfaches:                                   $\text{kgV}(a, b) := \min\{m \in \mathbb{N} : a \mid m, b \mid m\} = \prod_{p \in \mathbb{P}} p^{\max\{\nu_p(a), \nu_p(b)\}}$  
$a$ und $b$ sind teilerfremd (koprim):                                    $\text{ggT}(a, b) = 1$
$a$ mod $n$:                                                                           $a\%n = a - \left\lfloor \frac{a}{n} \right\rfloor n = r\in \{0,n-1\}, a\equiv_n r$

### ggT
größter gemeinsamer Teiler: 
für $a, b \in \mathbb{N},0< a<b$
$\text{ggT}(a, b) := \max\{d \in \mathbb{N} : d \mid a, d \mid b\} = \prod_{p \in \mathbb{P}} p^{\min\{\nu_p(a), \nu_p(b)\}}$  

$\text{ggT}(0, a) = |a| \quad \text{und} \quad \text{ggT}(1, a) = 1.$  
$\text{ggT}(a, b) = \text{ggT}(|a|, |b|) \quad \text{und} \quad \text{ggT}(a, b) = \text{ggT}(b, a).$  
$\text{ggT}(a, b) = \text{ggT}(a, a + b) = \text{ggT}(a, a - b).$  
$\text{ggT}(a, b) = \text{ggT}(a, b - \lfloor b / a \rfloor a) = \text{ggT}(b \mod a, a)$
⇒ ggT Algorithmus ohne Primfaktoren

### Restklassen und $\equiv_n$
$a$ und $b$ haben selben "Rest" bei Division durch $n$:
$a \equiv_n b \iff n \mid (b - a) \iff \frac{b - a}{n} \in \mathbb{Z} \iff b - a \in n\mathbb{Z} \iff (a\%n)=(b\%n)$

Äquivalenz-/Rest-klassen: $[a]_n := \{a + nz \mid z \in \mathbb{Z}\} =: a + n\mathbb{Z}$
Standard Repräsentantensystem: $\mathbb{Z}_n := \{0, 1, \dots, n - 1\}$
Quotient: $\mathbb{Z} / n\mathbb{Z} := \mathbb{Z} / \equiv_n = \{r + n\mathbb{Z} \mid r \in \mathbb{Z}_n\}.$
### Rechenregeln
$|a \cdot b| = \text{kgV}(|a|, |b|) \cdot \text{ggT}(|a|, |b|)$  

$a\mathbb{Z} \cap b\mathbb{Z} = \text{kgV}(|a|, |b|)\mathbb{Z} \text{ mit } m\mathbb{Z} := \{mk : k \in \mathbb{Z}\}$  

$a\mathbb{Z} + b\mathbb{Z} := \{ka + lb \mid k, l \in \mathbb{Z}\} = \text{ggT}(|a|, |b|)\mathbb{Z}$  

$\equiv_n$ ist mit $+$ und $\cdot$ verträglich, d.h. aus $a \equiv_n a'$ und $b \equiv_n b'$ folgt  
$a + b \equiv_n a' + b' \equiv_n (a + b) \mod n \quad \text{und} \quad a \cdot b \equiv_n a' \cdot b' \equiv_n (a \cdot b) \mod n$

⇒ Falls $[a]_n = [a']_n$ und $[b]_n = [b']_n$, dann  
$[a + b]_n = [a' + b']_n = [(a + b) \mod n]_n \quad \text{und} \quad [a \cdot b]_n = [a' \cdot b']_n = [(a \cdot b) \mod n]_n$  

⇒ Addition und Multiplikation von Restklassen: 
$[a]_n + [b]_n := [a + b]_n \quad \text{und} \quad [a]_n \cdot [b]_n := [a \cdot b]_n$

### Teilbarkeitsrelation
⇒ [[Hasse Diagramm]] des _Teilerverbands_ von $n = 360$
![[Pasted image 20250127155252.png]]
$\text{kgV}(a, b):$ kleinste Zahl, die von $a$ und von $b$ erreicht werden kann.  
$\text{ggT}(a, b):$ größte Zahl, die $a$ und $b$ erreichen kann.  

