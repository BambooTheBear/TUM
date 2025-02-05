Fragestellg: $x$ Objekte in $y$ Mengen aufzuteilen, sodass alle Mengen Y: $|Y|\geq 1$
⇒ z.B. 7 Geschenke auf 4 Kinder aufteilen

# Stirlingzahlen 2. Art $S_{n,k}$
## Objekte unterscheidbar, Mengen unterscheidbar  $F_{n,k}$
Möglichkeiten $k$ Objekte in $n$ (nicht leere) [[Mengen]] aufzuteilen
⇒ $F_{n,k}$
⇒ $|F_{n,k}| = n!\cdot S_{k,n}$ = $\sum_{i=0}^n (-1)^{n-i} \binom{n}{i} i^k$
## Objekte unterscheidbar, Mengen nicht unterscheidbar $S_{n,k}$
Anzahl der [[Potenzmenge#Partitionen|Partitionen]] von $n$ Elementen in $k$ (nicht leere) Klassen
⇒ $S_{n,k}$
⇒ $S_{n,k} = S_{n-1,k-1} + k \cdot S_{n-1,k} \quad \text{für } n > k > 0$
	$S_{n,0} = 0 \quad \text{für } n > 0$
	$S_{n,n} = 1$ 
>[!warning] Achtung!
>bei $F_{n,k}$ ist $k$ die Anzahl der Objekte auf die $n$ Mengen, bei $S_{n,k}$ umgekehrt!

## Objekte nicht unterscheidbar, Mengen schon (MINDESTENS 1)
⇒ $G_{n,k}$
⇒ $G_{n,k}= \binom{n-1}{k-1}$

## Objekte nicht unterscheidbar, Mengen nicht unterscheidbar (Mindestens 1)
$\vert P_{n,k} \vert = \vert P_{n-1,k-1} \vert + \vert P_{n-k,k} \vert \quad \text{für } k > 0$  
$\vert P_{n,0} \vert = 0 \quad \text{für } n > 0$  
$\vert P_{n,k} \vert = 0 \quad \text{für } k > n$  
$\vert P_{n,n} \vert = 1$

## Objekte nicht unterscheidbar, Mengen nicht unterscheidbar (NICHT min. 1)
⇒ $H_{n,k}=P_{n+k,k}$
# Stirlingzahlen 1. Art $s_{n,k}$ //TODO genau anschauen
⇒ Anzahl der [[Permutationen]] $[n]$ mit genau $[k]$ Zyklen
$s_{n,k} = \left[ \begin{array}{c} n \\ k \end{array} \right]$
//Todo formel
# Rekursion
Stirlingzahlen und der [[Binomialkoeffizient]] folgen dem selben Muster:
$\left[ \begin{array}{c} n+1 \\ k \end{array} \right]$   $=$  $\left[ \begin{array}{c} n \\ k-1 \end{array} \right] + n \cdot \left[ \begin{array}{c} n \\ k \end{array} \right]$ $\quad \text{ mit } \left[ \begin{array}{c} n \\ n \end{array} \right] = 1, \, \left[ \begin{array}{c} n+1 \\ 0 \end{array} \right] = 0$
$\left\{ \begin{array}{c} n+1 \\ k \end{array} \right\} = \left\{ \begin{array}{c} n \\ k-1 \end{array} \right\} + k \cdot \left\{ \begin{array}{c} n \\ k \end{array} \right\} \quad \text{mit } \left\{ \begin{array}{c} n \\ n \end{array} \right\} = 1, \, \left\{ \begin{array}{c} n+1 \\ 0 \end{array} \right\} = 0$
$\left( \begin{array}{c} n+1 \\ k \end{array} \right) = \left( \begin{array}{c} n \\ k-1 \end{array} \right) +$   $\quad \left( \begin{array}{c} n \\ k \end{array} \right) \quad \text{mit } \left( \begin{array}{c} n \\ n \end{array} \right) = 1, \, \left( \begin{array}{c} n+1 \\ 0 \end{array} \right) = 1$
