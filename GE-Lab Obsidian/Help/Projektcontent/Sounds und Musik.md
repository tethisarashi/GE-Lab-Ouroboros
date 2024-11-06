- Projekt über Fork geben
- mit Steffen noch klären, ob er Sounds in UE-Projekt einpflegt

### Soundliste

| **Sound**                                     | **Beschreibung/für was**                                 | **Requested von** |
| --------------------------------------------- | -------------------------------------------------------- | ----------------- |
| laufen menschlich                             | Trupp + NPCs                                             | Natalie           |
| Schwert schwung/angriff                       | Angriff im Kampf                                         | Natalie           |
| Axt schwung/angriff                           | Angriff im Kampf                                         | Natalie           |
| Bogen spannen + schießen                      | Angriff im Kampf                                         | Natalie           |
| Armbrust spannen + schießen                   | Angriff im Kampf                                         | Natalie           |
| Zauberspruch murmeln                          | Mit Effekten als Angriff mit Zauberbuch                  | Natalie           |
| Zauberspruch murmeln                          | Mit Zauberstab auf Boden schlagen                        | Natalie           |
| Keule schwung/angriff                         | Angriff im Kampf                                         | Natalie           |
| Dolche schnell zustechen                      | Angriff im Kampf                                         | Natalie           |
| schaden bekommen menschlich                   | Im Kampfmodus                                            | Natalie           |
| sterben mensch                                | Im Kampfmodus                                            | Natalie           |
| Wolf heulen                                   | ab und zu als Hintergrundgeräuch                         | Natalie           |
| Wolf knurren                                  | regelmäßig wiederholt im Kampf                           | Natalie           |
| Wolf beißen                                   | Angriff im Kampf                                         | Natalie           |
| Wolf jaulen                                   | Wolf bekommt schaden                                     | Natalie           |
| Wolf sterben                                  | Im Kampf                                                 | Natalie           |
| Mutant murren                                 | menschliches Murmeln regelmäßig im Kampf                 | Natalie           |
| Mutant schreien                               | tief, heiser, menschlich Angriff im Kampf                | Natalie           |
| Mutant schmerz                                | bekommt schaden                                          | Natalie           |
| Mutant sterben                                | Im Kampfmodus                                            | Natalie           |
| Holz knarzen                                  | lebender alter Baum der sich bewegt                      | Natalie           |
| Holz hacken                                   | Baum bekommt Schaden                                     | Natalie           |
| Holz spalten                                  | Baum stirbt                                              | Natalie           |
| Huhn gackern + Ziege mähen                    | friedlich, ab und zu als Hintergrundgeräusch             | Natalie           |
| Huhn + Ziege aggressiv durcheinander schreien | Angriff im Kampf, zu einem Hybrid mutiert                | Natalie           |
| Huhn + Ziege schmerz                          | bekommt schaden                                          | Natalie           |
| Huhn + Ziege sterben                          | Im Kampf                                                 | Natalie           |
| Holzrad rattern/knarzen + Pferd laufen        | für Wagen fahren, leichte Geräusche                      | Natalie           |
| Wagen rattern + Pferd wiehern                 | Wagen bekommt Schaden, stärkeres Geräusch                | Natalie           |
| Holzrad knarzen                               | Wagen anfahren, langsamer Anfang mit Übergang zum fahren | Natalie           |
| Holzrad knarzen + Pferd wiehern               | Wagen stoppen, Übergang von fahren                       | Natalie           |
| Menschen plaudern                             | NPCs, unverständlich im Hintergrund                      | Natalie           |
| Holz hacken                                   | NPC, im Hintergrund (kann auch selbes wie bei Angriff)   | Natalie           |
| Holzkurbel drehen                             | NPC, Wasser an Brunnen holen                             | Natalie           |
| Mensch schleichen                             | NPC, im Hintergrund                                      | Natalie           |
| Mensch murmeln                                | NPC, Zaubersprüche aus Buch versuchen                    | Natalie           |
| Münzen klimpern                               | NPC, Geld zählen                                         | Natalie           |

## Brainstorming
**Reihenfolge**
--> Overworld, Cart-Mode als erstes
--> Musik
--> Stadt
--> Handel/Dialog
--> UI
--> Kampf-, Gegner- und Waffensounds
--> POI
##### Cart-Mode (Fahren, Ressourcenmanagement, ...)
- Fahrt
	- Räder auf Erde
	- Räder auf Brücke (Steinbrücken, Holzbrücken)
	- Hufe auf Erde
	- Hufe auf Brücke (Steinbrücke, Holzbrücke)
	- Wagen rumpelt
		- Töpfe klimpern
		- Knarzen von Holz
		- Metall-Quietschen
- Wagen steht
	- Pferd schnauft
- Losfahren
	- Peitschen
	- "Hü"-Sound vom "Kutscher"
- Anhalten
	- "Ho"-Sound vom "Kutscher"
##### Kampf
- Bogen schnalzen und spannen (ein Sound!)
- Schwertschlag --> "Wusch"
- Schlag auf Schild --> "Donk"
- Schadensounds (Schaden bekommen)
	- Gegner nehmen Schaden entsprechend ihrer "Klasse"
		- Banditen
		- Wolf
		- Pflanze
		- Humanoider Mutant
		- Mutant Ziege-Huhn
	- Trupp Schadensounds humanoid
- Angriffsound (Angriff ausführen) --> Sound abhängig nach Waffe (falls Gegner eine Waffe hat, gibt auch nichtmenschliche Gegner)
	- Gegner (Steffen Gegner zeigen, bevor er Sounds dazu macht)
		- Waffensounds (Schwert, Schild, Bogen)
		- Wolf heult
		- Wolf knurrt
		- Wolf beißt
		- Pflanze peitscht
		- Pflanze tiefes Knarzen --> siehe Ents
		- Pflanze aggressives Blätterrascheln --> Grsssch 
		- Ziege mäht
		- Huhn gackert
		- Ziege mäht aggressiv
		- Huhn gackert aggressiv
		- Huhn-Ziege-Mutant Mischung aus Mähen und Gackern verzerrt
		- Humanoider Mutant keucht (wie TLOU Stalker/Runner)
		- Humanoider Mutant schreit (wie TLOU Stalker/Runner)
		- Humanoider Mutant keucht (wie TLOU Stalker/Runner) aggressiver als bisher
		- Humanoider Mutant schreit (wie TLOU Stalker/Runner) aggressiver als bisher
	- Trupp
##### Stadt
##### POI
##### Handel/Dialog
##### Overworld
- Wind in Blättern (Bäume)
- Vogelgezwitscher
- Wasser plätschert (Bach)
- Äste knacken (Ast auf Boden, man tritt drauf --> wie beim durch Wald laufen)
- Bäume knarzen 
- Gebüsch knackt und raschelt (wie wenn Tier wegläuft)
- Krähen krähen
##### Trupp
##### UI
- Items aufheben (in Inventar)
- Items ablegen (in Inventar)
- Bestätigen (Knopf-Sound)
- Inventar öffnen, z.B. Truhe-geht-auf-Sound (Knarz) --> im Cart-Mode
- Inventar schließen, z.B. Truhe-schließt-Sound (Plonk) --> im Cart-Mode
- Loot öffnen
	- Truhe öffnen
	- Kisten öffnen
	- Sack öffnen
	- Mittelgroße Steine beiseite schieben --> Loot  darunter
- Charakter isst --> Schmatzen, o.Ä.
- Charakter trinkt --> Runterschlucken
- Charakter heilt sich --> Heilsound
- Waffe ausrüsten, z.B. Klink 
- Item aus Inventar wegwerfen --> z.B. dumpfes Klonk
- Items verwerten --> Komplexe Objekte zerteilen in Handwerkswaren
##### Musik