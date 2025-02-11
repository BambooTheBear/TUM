Idee: Aufteilung von einem Cycle im [[_riscv_single.png|Single Cycle Prozessor]] in mehrere kleine Teilschritte ⇒ höhere/schnellere Taktfrequenz möglich aber eine Instruktion braucht mehrere Taktzyklen
⇒ Wieso? Mann könnte dann einzelne (längere) Teilschritte "überspringen" statt auf ihre potenziell benötigte Ausführung in der langen Taktfrequenz zu warten
	- z.B. ist die Taktfrequenz im Single Cycle Prozessor die längste mögliche Operation (höchster kritischer Pfad der ganzen Schaltung) ⇒ Daten im [[Hauptspeicher]] laden/speichern ⇒ selbst ein einfaches JUMP braucht die Taktfrequenz vom Haupspeicher ⇒ ineffizient
	- ein Multi Cycle Prozessor könnte einfach sagen: "Ah ok du willst nur jumpen? das braucht 3 kurze Takte, ah du willst laden? das braucht lange weil ich muss erst deine adressen holen, dann mit dem immidiate verrechnen, dann aus dem hauptspeicher ziehen und dann noch in die Register laden ⇒ x Taktzyklen" ⇒ Potentieller Speedup, ABER: jede Taktfrequenz immernoch die höchste mögliche Länge eines Teilschrittes (Jeder Taktzyklus muss gleich lang sein!)
	
⇒ Umsetzung der einzelnen _Zuständen_ (aka welcher Teilschritt gerade) durch [[Endliche Automaten|einen endlichen Automaten]] im Steuerwerk ([[Control Unit]])
⇒ Damit die Daten zwischen den Zuständen nicht verloren gehen oder "zu früh" propagiert werden, Clockgesteuerte [[D-Latch]] zwischen jedem "Teilschritt"
⇒ so unnötig komplex bei kaum (oft gar keinem/negativen) Speedup dass sie sich nicht umgesetzt haben
![[_riscv_multicycle.png]]
