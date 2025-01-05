Ein [[Graphen|Graph]] ist _planar_ gdw. man ihn _ohne sich überschneidende Kanten_ auf einer 2D Fläche aufmalen könnte

## Eulersche Polyederformel
Ein [[Graphen#Eigenschaften|zusammenhänder]], planarer Graph teilt die Zeichenebene in $f$ Flächen auf mit
$f-|E|+|V|=2$

Für jeden planaren Graphen mit k [[Graphen#Eigenschaften|maximalen Zusammenhangskomponenten]] gilt
$f-|E|+|V|=1+k$

## Satz von Kuratowski
der [[Graphen#vollständiger bipartiter Graph $K_{m,n}$|K_3,3]] und der [[Graphen#Vollständiger Graph $K_n$|K_5]] sind **nicht** planare Graphen
_Satz von Kuratowski:_ ein einfacher Graph ist planar gdw. weder der $K_{3,3}$ noch der $K_5$ ein _Minor_ von ihm sind
### Minor
Ein Graph $H$ ist ein Minor von Graph $G$ wenn man mittels
- Entfernen von Kanten
- Entfernen von Knoten mit Grad 0
- Kantenkonraktion ⇒ man enfernt eine Kante $\{u,v\}$ und verbindet alle Nachbarn von $u$ mit $v$ und entfernt anschließend $u$
aus $G$ $H$ machen kann 