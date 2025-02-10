Wenn eine Architektur/System/Angabe im _Zweierkomplement_ arbeitet:
### $n_2$ negativ machen
Flippe alle Bits und addiere dann 1
### $-n_{10}$ in Binär
Konvertiere $n$ zu binär und (da negativ) dann ins zweierkomplement
### $n_2$ im Zweierkomplement zu $n_{10}$ (Dezimal)
Wenn _höchstes Bit_ (MSB) = 0, Zahl ist definitiv positiv/null ⇒ einfach konvertieren
Wenn MSB = 1, Zahl ist neagtiv ⇒ Alle bits flippen, 1 addieren ⇒ resultat einfach konvertieren, "minus" davorsetzen

⇒ Das Zweierkomplement von einer Zahl im Zweierkomplement ist "das positive" der Zahl, da -(-n) = n