[[Potenzen]] von [[Gruppe|Gruppen]] können auch als [[Graphen]] dargestellt werden
Jedes $a \in \mathbb{G}$ definiert eine [[Permutationen|Permutation]] $r_a(x) = xa$ und damit einen Graph der alle Elemente als Knoten und als Kanten alle Abbildungen die sich durch die Zyklen aus der Permutation ergeben.
## Beispiel $(\mathbb{Z}_9^*, \cdot_9, 1)$
[[Gruppe#Cayley table|Cayley Table]] zu  $(\mathbb{Z}_9^*, \cdot_9, 1)$

| $\cdot_9$ | 1 | 2 | 4 | 5 | 7 | 8 |
|-----------|---|---|---|---|---|---|
| 1         | 1 | 2 | 4 | 5 | 7 | 8 |
| 2         | 2 | 4 | 8 | 1 | 5 | 7 |
| 4         | 4 | 8 | 7 | 2 | 1 | 5 |
| 5         | 5 | 1 | 2 | 7 | 8 | 4 |
| 7         | 7 | 5 | 1 | 8 | 4 | 2 |
| 8         | 8 | 7 | 5 | 4 | 2 | 1 |
### Erzeuger 2$\langle 2 \rangle$
$\langle 2 \rangle := (1,\quad 1\cdot_9 2,\quad1\cdot_9 2\cdot_9 2,\quad1\cdot_9 2\cdot_9 2 \cdot_9 2,\quad 1\cdot_9 2\cdot_9 2 \cdot_9 2 \cdot_9 2,\quad 1\cdot_9 2\cdot_9 2 \cdot_9 2 \cdot_9 2 \cdot_9 2 )$
	$:= (1,\quad\quad2,\qquad4,\qquad\qquad\quad8,\qquad\qquad\qquad7,\quad\quad\quad\quad\quad\quad\quad\quad5)$

![[Pasted image 20250205145642.png]]

### Erzeuger 4$\langle 4 \rangle$
$\langle 2 \rangle := (1,\quad 1\cdot_9 4,\quad1\cdot_9 4\cdot_9 4),\qquad(2,\quad 2\cdot_9 4,\quad2\cdot_9 2\cdot_9 2)$
	$:= (1,\quad\quad4,\qquad7),\qquad\qquad(2,\qquad8,\quad\quad\quad\quad5)$
![[Pasted image 20250205150002.png]]
