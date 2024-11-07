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
	- Trupp Schadensounds humanoid --> 4 verschiedene: z.B. alt, leidend, aggressiv, ... --> 4 verschiedene für 4 verschiedene Charaktere von 4 verschiedenen Fraktionen 
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
		- restliche Waffen siehe Gegnerangriffsounds
		- Magieangriff mit magischem Stab von Magier
		- Magieangriff mit Buch, z.B. Zauberspruch murmeln
		- Axt
		- Armbrust
		- Dolch
		- Keule/Stock
		- HUA-Geräusch z.B. in alt, heroisch, aufgeweckt, aggressiv, ... --> 4 verschiedene für 4 verschiedene Charaktere von 4 verschiedenen Fraktionen 
##### Stadt
- Markt-Geräusche (nicht zu positiv, eher neutral, keine lachenden Leute im Hintergrund o.Ä.)
- Kirchenglocke
##### POI
- Fensterscharnier knarzt (kaputtes Fenster im Wind, verlassenes/kaputtes Haus)
- Einzelner Stein fällt auf Stein (Ziegelstein fällt auf Ziegelstein, z.B. bei Ruine, Kieselstein geht auch --> soll das Feeling geben, dass Umgebung brüchig ist)
- Wind zieht durch verlassenes Gebäude 
- Einzelner Wassertropfen in Höhle tropft auf Boden
- Magiegeräusch --> ominöses Rauschen, wabbernder Sound --> Riss im Boden, leuchtet lila raus, viel Macht breitet sich aus
- Magiegeräusch für Flüssigkeit --> ominöses Wabern, Rauschen --> magische Flüssigkeit rauscht in einer Art Gefäß
- Altes Windrad quietscht im Wind --> Windrad wie auf amerikanischer Farm --> aus Metall oder Holz
##### Handel
- Gold klimpert --> Handel bestätigen
##### Dialog
- Schriftrolle rollt auf
- Dada-Sound, wenn Quest angenommen wird
- Neutrales Murmeln für Dialog 
- Positives Murmeln für Dialog
- Negatives Murmeln für Dialog
##### Overworld
- Wind in Blättern (Bäume)
- Vogelgezwitscher
- Wasser plätschert (Bach)  
- Äste knacken (Ast auf Boden, man tritt drauf --> wie beim durch Wald laufen)
- Bäume knarzen 
- Gebüsch knackt und raschelt (wie wenn Tier wegläuft)
- Krähen krähen
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
- Kampfmusik: "aggressive", mittelalterliche Musik mit Gitarre und Tamburin 
	- Referenz, KEINE VORLAGE, schon fertige Musik nicht wegwerfen: https://www.youtube.com/watch?v=U4GmjvjB2Rw&list=PL7FVc5pl0q2MSCbRTByCy1Wy4N6ITcacy&index=2
- Overworld-/Reisemusik und Stadtmusik
	- Referenz, KEINE VORLAGE, schon fertige Musik nicht wegwerfen: https://www.youtube.com/watch?v=GVjwJxYDJUA
	- Referenz, KEINE VORLAGE, schon fertige Musik nicht wegwerfen: https://www.youtube.com/watch?v=tGl4FLMp2Hg
	- Referenz, KEINE VORLAGE, schon fertige Musik nicht wegwerfen: https://www.youtube.com/watch?v=8oCO_yGtO40
- Overworldmusik/Reisemusik: Hintergrundmusik für Reise, melancholische Musik
-  Stadtmusik: eher ruhig, Gefühl von Ausruhen