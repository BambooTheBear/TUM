Karnaugh-Veitch-Diagramm (⇒  [[KV Diagramme]]) der boolschen Funktion und dann "zusammenfassen" von $2^n*2^m$ großen Rechtecken (Päckchen), 
ver-[[AND]]-en der Variablen die sich _nicht_ verändern und dann verodern aller [[Literale]]
![[Pasted image 20250212113716.png]]

## Logik-Hazards
wenn Funktion durch K-Map zu Schaltkreis umgewandelt wurde, können durch Länge von [[Critical Path]]s Logik Hazards (Flakern) enstehen, die dann z.B. [[D-Latch]]e zerstören können.
⇒ Vermeidung durch "unnötige" Literale aus dem KV Diagramm hinzufügen ⇒ JEDE AN EINE 1 Angrenzende 1 MUSS MIT DIESER IN EINEM LITERAL SEIN ⇒ Blaue Markeirung im obigen Bild