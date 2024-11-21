### Kampf:
- auf Pfad, d. h. Wagen hält an, Charaktere und Gegner werden gespawnt und entsprechend aufgestellt, Kamera von Seite
- "Münze werfen" wer anfangt (d. h. Zufallszahl%2 == 0 oder != 0) --> geht dann immer hin und her, d. h. ein Gegner ein Trupp ein Gegner ein Trupp etc --> beide Parteien werden der Reihe nach durchgegangen
- Kampf dauert Anzahl Runden/2 Ticks
- Trupp ist am Zug: Kampfaktionen des Charakters, der an der Reihe ist, werden angezeigt + Möglichkeit zur Heilung 
- Gegner auswählen und Kampfaktion durchführen oder halt heilen (dann kein Gegner auswählen)
- Wenn Gegner am Zug: Gegner wählt zufällig Charakter aus Trupp aus und führt Attacke aus ODER heilt sich zu gewisser Chance (Gegner soll sich nicht immer instant heilen sobald er unter gewissen Healthwert fällt)
- Wenn alle aus Trupp tot: Game Over
- Wenn alle aus Gegnerteam tot (sofern es mehrere Gegner im aktuellen Kampf gibt): Alle Überlebenden despawnen bzw. in Karren zurück spawnen, Tickcounter entsprechend erhöhen, Kamera wieder auf Third-Person-Modus, auf W weiterfahren können (bool isFighting, um sämtliche Fahrtaktionen zu blockieren)

### Essenzielle Schritte:
- Loop für Hin und Her im Kampf (Länge einer Runde = max(Anzahl Truppmitglieder, Anzahl Gegner) lang, d. h. Rundencounter % Rundenlänge
- Mechanik für hin und her
- Mechanik für Auswählen der Charaktere, die von Gegner angegriffen werden sollen --> möglichst random
- Mechanik für Heilen und Auswahl Angriff auf Gegnerseite
- Handlungen des Trupps werden von Spieler bestimmt
- Wenn Heiltrank im Inventar leer, kein Heilen im Kampf möglich --> siehe Fragen

#### Fragen
- Kann man nur den Charakter heilen, der dran ist oder einen beliebigen?
- Wird Angriff irgendwie verrechnet? Rüstung, Blocken, etc?
- Was ist mit Blocken? Automatisch Blocken mit gewisser Chance?
- Wie kann man die Auswahl der anzugreifenden Charaktere aus dem Trupp (von Gegnerseite aus) möglichst random machen? bzw. wann genau soll sich ein Gegner heilen? Welche Chance?
- Heiltrank abhängig von Inventar?

### Scribbles

![[Pasted image 20241121185323.png]]![[Pasted image 20241121185341.png]]