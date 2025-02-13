Ein Endlicher Automat repräsentiert eine Funktion die zwischen Zuständen übergeht,
Mathematische Beschreibung als 6-Tupel $(I, O, S, s_0, \delta, \lambda)$:

- $I$: Menge möglicher Eingaben  
- $O$: Menge möglicher Ausgaben  
- $S$: Zustandsmenge  
- $s_0$: Startzustand  
- $\delta: S \times I \to S$: Zustandsübergangsfunktion  
- $\lambda: S \to O$ (Moore), $\lambda: S \times I \to O$ (Mealy): Ausgabefunktion  

## Moore (Ausgabe abhängig vom Zustand)
![[Pasted image 20250211212218.png]]

## Mealy (Ausgabe abhängig von Zustand und Eingabe)
![[Pasted image 20250211212243.png]]

# Kodierung
## One Hot Kodierung
Ein D-Latch pro Zustand, Übergang mit einfacher vergatterung zum nächsten Zustand ⇒ Einfach und ablesbar ⇒ schnell sehr komplex
![[Pasted image 20250211212457.png]]

## Binär Kodierung
Zustände werden Binär kodiert und dann "hard-codet" in einen Art Truth Table basierend auf inputs ⇒ nicht einfach ablesbar
![[Pasted image 20250211212618.png]]
## Mikroprogrammiertes Steuerwerk
Einfach ein hardcoded Branch if Condition, Increment "PC"/nächste Addresse +1 über Multiplexer
![[Pasted image 20250211212713.png]]
