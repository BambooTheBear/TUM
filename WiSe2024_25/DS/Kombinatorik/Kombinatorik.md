_Kombinatorik_ bezeichnet die _Anzahl der verschiedenen Möglichkeiten_ die ein Ereignis haben kann
⇒ z.B. _Möglichkeiten_ eine Hand in Poker zu ziehen

## Grundregeln
### Summenregel
$\lvert A \cup B \rvert = \lvert A \rvert + \lvert B \rvert - \lvert A \cap B \rvert$
### Produktregel
$\lvert A \times B \rvert = \lvert A \rvert \cdot \lvert B \rvert$
### Urbildregel
Wenn es eine [[Funktionen von Mengen|Abbildung]] $f: A\rightarrow B$ mit $|f^{-1}(b)=m$ mit konstantem $m$ für alle $b \in B$ dann gilt $|A|=m*|B|$
### Schubfachprinzip
Wenn $n$ Objekte in $k$ Boxen platziert werden, dann gibt es mindestens eine Box mit $\lceil n / k \rceil$ Objekten.
### Zählregel
$\sum_{s \in S} \lvert \{t \in T \mid (s,t) \in R\} \rvert = \sum_{t \in T} \lvert \{s \in S \mid (s,t) \in R\} \rvert$
⇒ Bei einer Tabelle ist es egal ob man alle Zeilen aufsummiert oder alles spalten...