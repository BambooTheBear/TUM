Compiler möchte minimal viele Register verwenden ⇒ [[Knotenfärbung]]s Problem:
Notation aller Register und wie lange sie nicht überschrieben werden dürfen (wegen [[Pipeline Konflikte#Datenabhängigkeiten|Datenabhängigkeiten]]) ⇒ Notation am ende nicht mehr miteinbeschlossen
z.B.
![[Pasted image 20250212135039.png]]

Dann Knoten für alle Register im [[Graphen]] erstellen und alle Knoten Paarweise verbinden wenn sie an mind. einem Schritt gleichzeitig benötigt werden
⇒ 
![[Pasted image 20250212135300.png]]
Dann Knotenfärbung berechnen, Anzahl an benötigten Färbungen = Anzahl benötigter Register
⇒ 
![[Pasted image 20250212135338.png]]
