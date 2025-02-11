Ein Chache Besteht aus einer Anzahl an Tag-Cachezeilen Paaren
⇒ Der Tag ist ein Teil einer Adresse (meistens 32 Bit groß, gespeichert in z.B. Registern) die auf ein Datum im [[Hauptspeicher]] zeigt (z.B. ein 4Byte Int in der RAM)
⇒ Das referenzierte Datum im Hauptspeicher wird dann zusammen mit allen umliegenden Daten ([[Lokalität|örtliche Lokalität]]) in die jeweilige _Cachezeile_ geladen
⇒ Cachezeilen können in _Cachesets_ grupiert werden ⇒ n-Cachezeilen pro Cacheset ⇒ _n-assoziativer Cache_

Offset Bits = $log_2(\frac{\text{Cachezeilengröße}}{\text{Cachezeilen Alignment (meistens 1)}})$ = hintersten Bits ⇒ Geben an wo in der Cachezeile das tatsächlcihe Datum gespeichert wird
Index Bits = $\lceil log_2(\text{Anzahl der Cachesets})\rceil$ = bits vor Offsetbits ⇒ Geben an welches Cacheset betroffen ist
Tag Bits = Restlichen Bits ⇒ Identifizieren die in der Cachezeile gespeicherten Daten

![[Pasted image 20250211161636.png]]

# Direct Mapped Cache
1-assoziativ ⇒ Jedes Datum kann direkt auf eine Cachezeile gemapped werden ⇒ sehr schnell ⇒ oft Verdrängungen
# Vollassoziativer Cache
1 Cacheset das dann _Anazhl-Cachezeilen_-Assoziativ ist ⇒ Keine "unnötigen" Verdrängungen ⇒ sehr langsam (Überprüfung jedes einzelnen Tag Bits)
# n-assoziativer Cache
Mischform mit x Cachesets à n Cachezeilen ⇒ n-assoziativ