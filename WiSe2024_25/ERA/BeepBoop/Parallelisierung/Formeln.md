Mit $t_s$ sequentieller Programmteil, $t_p$ paralleler Programmteil, $n$ Anzahl CPU-Kerne, $T$ Ausführungszeit mit $n = 1$:

⇒  **Amdahlsches Gesetz:** Gleiche Problemgröße, aufgeteilt auf mehrere Kerne → begrenzt durch sequentiellen Anteil  
$S_{\text{Amdahl}}(n) = \frac{T}{t_s + \frac{t_p}{n}}$  

⇒  **Gustafsons Gesetz:** Mehr Kerne können mehr berechnen: Größeres Problem → paralleler Anteil wächst mit Problemgröße, $t_s$ proportional kleiner  
$S_{\text{Gustafson}}(n) = \frac{t_s + n \cdot t_p}{T}$
