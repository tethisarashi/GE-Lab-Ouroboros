##  Fragen:
- inzwischen alle geklärt.

- Plakat abstimmen => mach ich dann
- Karo schreiben welche BP_Anim wo rein muss
- Ob wir zusammen Tabelle wer was gemacht hat oder jeder einzeln in Doku -> alle selbe tabell nach unserer Obsidian liste => machen Google Docs die zusammen und jeder kopiert sich die dann
- Ob wir ressourcen einzeln oder als gruppe -> da abgabe dass ihn zu github hinzufügen -> was die meinen, was man da noch "abgeben" muss => ihn einfach hinzufügen und in readme noch was rein schreiben
- Dass ich Bühling verstehen kann mit seinem "Game Loop" -> also was Ziel und was Weg dorthin -> Ob wir dafür am anfang Text einblendung machen (etwas hässlich, aber geht am schnellsten), hätte 2 vorschläge für Text (beide eher noch änderbar) => wird gemacht, entweder einer meiner Texte, oder robin macht da was
- und ob dann zweites Pop-Up (vielleicht kurz in oberer Bildschirmecke) mit zB "TAB for Controlles" und mit TAB dann nur ein/ausblenden von Controlles Overlay -> wäre besser das in menü zu haben (mit dem man auch zurück zu Startbilldschirm kommen würde, aber das haben wir ja alles nicht -> ob wir das noch einbauen => mit taste einblenden und Startmenü aber kein Pausenmenü
- hab die commits alle hässlich gemacht (sind jetzt alle doppelt gelistet) => alles gut solange nichts kaputt geht
- wer steht im kampf links und wer rechts -> Trupp steht links
- Ob Karo Waffe an hand Tracken kann, sonst mach ich jew immer extra mesh für Kampf Modus -> dann muss Karo aber das Mesh ändern für Kampf => Waffen meshes einzeln, Karo positioniert dann in Hand
- hätte gerne seperate ordner für mehses und materials und animation, oder ob lieber alles beisammen (karo muss ja finden können) => An den Link halten, so wie da aufgeteilt https://github.com/Allar/ue5-style-guide?tab=readme-ov-file#structure
- Karo über problem informieren, dass reimport evtl. schwierig/nicht möglich, weil bisher nur Mesh ohne Skelett => sollte passen wenn später austauscht, weil im Code das jew. aus den gegeben auswählt (un das geht auch im Nachhinein nochmal)
- Robin, ob eltern Material in Ordner Materials und nur instanzen in Unterordner -> ja, Grundmaterial in Order Materials und die Instanzen zu den Meshes
- Wie schnell ungefähr Wagen ist -> gemütlich lauffen nicht rennen
- wann immer mergen? nach jeder wochen task oder erst wenn quasi ganzen branch fertig -> erst wenn branch fertig => stages: Blockmehes, Meshes, Materials, Animationen, Texturen ==> für mitte bis ende Woche Besprechung ==> siehe unten, branch immer wieder mergen
- Wissen die anderen wie man das spiel deploied? Müssen wir das machen? => machen wir, bekommen wir schon hin, kümmern uns am Ende drum
- eher info: brauche für animation später in Code info welche waffe (nicht welcher char) => hab informiert -> muss selber noch recherchieren
- Wenn in animations Branch und mesh ändern will soll/muss nicht brach zu Models wechseln sondern einfch weiter mit in animationsbranch
- wie skeletal mesh scalen (Hund) => anschauen => alles an scaling anschauen/recherchieren (cart wurde im blueprint gescaled)
- wo Itemliste + wann -> später von robin in obsidian -> für waffenliste werte (schaden, preis, größe, beschreibung(offensichtlieche sachen wie bogen ist zweihändig))
- soll für Bandit auch 3 stages? aktuell hat nur eine genau wie hund -> passt so wies jetzt istsoll für Bandit auch 3 stages? aktuell hat nur eine genau wie hund -> passt so wies jetzt ist
- Wenn system wie jetzt brauche aus code viele bools für welche waffe und ob starker oder schwacher angriff (von angriff bool wenn event getriggert weil ich nicht auf event zugreifen kann) => bekomme ich von Karo
- soll ich erstmal nur so lassen (alles als keyframe animations -> räder + damage händisch -> dann brauche aber noch bool für hit) => ja soll erstmal so lassen
- in alle BP_BaseCharacter... jeweils in SK_... in Animation die BP_Anim_HumanChar rein
- zwischen bool true/false delay einbauen
- Ob Fight los geht und ob in Stadt steht
- Müssen ausprobieren, ob funktioniert, wenn die Trigger gleich heißen

----
## Aufgaben:
***Meshes:***
- Trupp (nach Fraktionen)
- Wagen (mit Pferd, Truhe, Kochstelle, empty space für langsam Füllen, Sitzen, Waffenhalterung) (Rad einzeln für Item)
- NPCs (nach Fraktionen (so 2/3 die dann mehrfach einfügen))
- Gegner (ca. 3-6 jew. 3 evolutions)
- Waffen (erstmal 1-2 pro Char) -> 3D Mesh + 2D Image davon

***Animationen:***
**-Trupp:**
- Idle -> sitzen + stehen + stehen kampf
- Walk
- Attack
- Hit
- Death

**-Gegner:**
- - " - (wie Trupp)

**-NPCs:**
- Idle/Random Stuff (Winken, Holzhacken o.ä.)

**-Wagen:**
- fahren
- damage
- start/stop


***Ideen:***
**-Gegner:**
- Wölfe
- Pflanzen (Stage 1 normal aber touchdamage, ab Stage 2 Monster)
- Mutanten (menschlich zu monster)
- Ziege + Huhn (stage 3 zu Hybridmonster)

-------------------------------------------------
# Workflows:
***-Obsidian:***
->Sourcetree + Obsidian öffnen
->in Sourcetree pullen (wenn nichts mehr offen ist, das noch commited werden muss)
-> zeug in Obsidian machen
-> in Sourcetree auf Commit -> das was geändert drauf drücken (stagen), Kommentar dazu schreiben -> commit (unten rechts)
-> dann pushen (sollte dann oben angezeigt werden, sofern keine Fehler geworfen werden)

***-Blender Blockmeshes:***
-> einfache Modells erstellen
-> Ordner in Unreal erstellen
-> Modells importieren

***-Blender Meshes final:***
-> Modells mit Rig erstellen
-> UV-Maps Prüfen
-> In Unreal importieren und prüfen
-> Wenn Zeit alle Rig Gewichtungen korrigieren

***-Animation:***
-> in Blender erstellen
-> in Unreal importieren
-> Animation BP erstellen

_________
# Timeline:

- (15.10.24) Blockmeshes Trupp, Gegner, NPC + fbx davon
- (18.10.24) Blockmeshes Wagen, Waffen + fbx davon
- (25.10.24) Mesh Cart ohne Rig
- (26.10.24) Rigged Mesh für Cart (Blender + fbx + UE)
- (01.11.24) Rigged Mesh für Base Human (blender + fbx + UE)
- (26.10.24-05.11.24) Materials Cart (Planken, Metall, Fell, Leder, Stoff, Haut)
- (05.11.24) Meshes Cart + Human fixed (UV Maps in Blender erstellt); Skelett Cart verbessert; Alle Master Materials + deren Instances für Cart + Human; dann alles von Karo, Robin und mir in Develop gemerget und Karo hat zusammengeführt => Cart fährt auf Spline auf Map
- (06.11.24) Fixed Materials Cart in Develop -> Materials waren nicht alle zugewiesen -> in Blueprint rein gehen und da dann zuweisen
- (08.11.24) Rigged Mesh für alle von Trupp mit UV (Blender + fbx)
- (09.11.24) Karo hat Soundliste vom Ergebnis der Besprechung aufgeschreiben, wir haben kontrolliert
- (09.11.24) Skeletal Meshes für alle von Trupp in Unreal importiert mit Materials
- (15.11.24) Rigged Mesh für alle Enemy Stage 1 (Bandit, Dog, Hybrid, Mutant, Plant, Wolf) + Mesh Weapons (Axe, Bow)
- (16.11.24) Mesh Weapons (rest) + Rigged Meshes alle Enemy mit Material in Unreal + Mesh Weapons mit Material in Unreal
- (22.11.24) Rigged Mesh Enemys (alle = Hybrid, Wolf, Mutant, Plant) in Stage 2 (Blender) + alles mit Materials in Unreal + Itemliste Weapons (noch nicht in Obsidian)
- (29.11.24) Rigged Mesh Enemys (alle) in Stage 3 (Blender)
- (30.11.24) Skeletal Meshes Enemys Stage 3 mit Materials in Unreal + Material Corruption + upated Textures and Normals (Paper, Fabric, Fur) + Rigged Meshes NPCs (alle) in Blender + mit Materials in Unreal
- (06.12.24) Animation Cart (Idle + Drive (without Wheels and damage)) in Blender + in Unreal
- (07.12.24) Animation Cart fertig (alles, als Keyframe Animation) in Blender + Unreal
- (13.12.24) Images von Chars und Waffen in UI_Art > Raw_Images + Itemliste mit vorläufigen Werten in Obsidian + Animationen Chars in Blender + Grundsetup für Unreal (aber funktioniert noch nicht richtig)
- (15.12.24) Animation Chars jetzt anderes System, Trigger definiert (Karo ruft dann auf), Animationen spielen aber noch nicht ab + Character Mesh Glitches Fixed Blender + Unreal
- (20.12.24) Animation Enemys (Bandit=Char|Hund=Wolf|Wolf=Alle Stages gleich|Mutant=jew. S, selbes SK|Plant=S2/3, selbes SK|Hybrid=jew. S, jew. SK) in Blender + imported in Unreal
- (21.12.24) Animation BPs mit Triggern definiert für Enemies (Karo muss noch aufrufen)
- (25.12.24-03.12.25?) Plakat
- (31.12.24) Conduits in Charakter Animations gefixt (Siehe Problem)
- (01.01.25) Fixed Bugs: Runtime Errors bei Enemy Animationen, dass Animationen aus kampf auch nach Ende des Kampfes fertig abgespielt wurden, Heal Animationen bei Enemy hinzugefügt (Blender + Unreal), Delays bei Animationen angepasst
- (06.01.25) NPC Animationen Blender + Unreal, Spieltitel Bild, Normal Maps Skalierung angepasst
- (08.01.25 - 10.01.25) Inventar Items zeichnen
- (09.01.5) Bugfix Error Messages Cart Animation meine Seite Versuch (Karo muss noch neu triggern)
- (17.01.25) Bug fix = Weight Paint Enemy Bandit, Obsidian Notizen hinzufügen, Code aufräumen


# Probleme:

->Allgemein: dass Dinge viel länger brauchen als gedacht + Kompatibilität + Recherche dauert auch lange

->Allgemein Kommunikation: z.B. (dass auch Bandit Gegner o.ä.)

-> Reimport von Mesh einfach möglich -> fraglich ob geht, da bisher in Blockmesh kein Rig 
=> sollte kein Problem, kann später austauschen, weil im Code das jew. aus den gegeben ausgewählt und das geht auch im Nachhinein

-> wie Riggen damit in unreal passt -> kann Räder in Blender nach Koordinaten drehen lassen, frage ob das auf UE übertragbar
=> Nein, nicht übertragbar, aber hab Mesh so mit Rig, dass steuerbar (Mesh unterteilt, einzeln Rigged, dann erst Mesh join)

-> wie eigene Textures (jew. Base Colour, Normal Map, Height, …) in unreal erstellen/importieren, die dann zum Mesh passen
=> evtl. in Blender Textur Materials machen (mit UV etc.), auf selbem Bild wie in UE, dann nochmal Exportieren ???
=> Tex in Krita malen (schwarz weiß, weiß wird ersetzt) + Blender UV map machen -> das ins Material in Unreal -> nein in Krita Filter für Normal Map

->materials nicht richtig funktioniert -> Rotation, Polygongrößen etc.
=> in Blender Mesh erst sinnvoll zerlegen (wenn nötig) dann Auto UV unwrap, da Anpassungen (falls nötig) dann mesh teile wieder Joinen -> dann alles auf einer UV Map, auch übereinander aber das ist egal, solange diese später andere materials haben

-> Cart ist Pawn und kein Character, deswegen funktionieren einige Funktionen der Animation nicht
=> anders gemacht bis optisch funktioniert
-> weil Pawn auch Physical Animation nicht so wirklich möglich/nicht so wie soll
=> sieht eh nicht ob Räder drehen oder nicht also egal?
==> für beides erstmal nur Keyframe Animation und das mit Physical auf Nice to Have verschieben

-> wenn in Funktion Bools true und wieder false setzt ist das zu schnell um es in Animation BP abzufragen und in Fkt kein delay möglich
=> definiere in Anim BP Trigger die mit delay true/false und die werden dann in Funktionen (zb in instandes von Chars) aufgerufen/ausgelöst

-> conduits in der state machine funktionieren immer nur in eine Richtung, nicht bidirectional. also kann zu Animation hinm aber nicht wieder zurück
=> ist bekannter (aber in dem fall wohl nicht gefixter) Bug in der Unreal Engine => jeweils immer 2 conduits, einen pro Richtung

-> geht mit BP nicht, dass zwei gleichzeitig an selben File arbeiten, weil die Binär Dateien sind, die kann man dann nicht mergen => wenn was von anderem Zuständigkeitsbereich braucht, muss das bei dieser Person anfragen


# Quellen:
=> wenn kopiert, dann als Quelle => "genau das aus Quelle XY übernommen und dann Z selber gemacht (Z nicht alle Notes erklären sondern die Idee)"
=> wenn zumindest benennen kann (z.B. diese 5 Videos) dann als Inspiration angeben => "Eingearbeitet in Unreal mit Videos XY"
=> für meine Methode bei Trupp: "Begriff Googlen und schnell runter scrollen" => angeben "Google Bildersuche [Suchbegriff]" (hier: Mittelalter Kaufmann; Bandit; Mittelalter Bauer; Drachenmagier)


-(26.10.24) Videos zu Blender Rigging: https://youtu.be/nMZOGWX4uMs?feature=shared (Quickly Rig Your Characters in Blender! von Thomas Potter)und https://youtu.be/jIwrswJEFBQ?feature=shared (Amazingly EASY Way To Rig Characters in Blender 4.1 von richstubbsanimation) (und https://youtu.be/3RSwjZLClRc?feature=shared (3D Rigging is Beautiful, Here's How It Works! von Doodley)) => Konzept mit Driver Bones übernommen und angepasst (an sich damit Wissen von früher aufgefrischt)

-(26.10.24-05.11.24) Eingearbeitet in Unreal Material Notes mit Videoplaylist: https://youtube.com/playlist?list=PLUi8nuTUEtTvrcISNaNpZwtxpQbyaBstT&feature=shared ("5-Minute Materials" von PrismaticaDev)

-(-"-) einfaches UV Scaling in Blender: https://youtu.be/bHbgQs8zkpw?feature=shared (How to Flatten UV Islands (Blender Tutorial) von Default Cube)=> Konzept von Island Scaling übernommen, aber nur ausgewählt für manche teile der Meshes angepasst

-(08.11.24) Google Bildersuche Mittelalter Kaufmann; Bandit; Mittelalter Bauer; Drachenmagier

-(07.12.24) Pawn Animation: https://youtu.be/z7WYuOf7tWs?feature=shared ("Spider Pawn #1 - Movements and Animations" von
	CodeLikeMe)
	Pawn Animation mit State Machine: https://youtu.be/daNOJlX1_8g?feature=shared ("THIS is how To use ANIMATION 	BLUEPRINTS in Unreal Engine" von The Game Dev Cave)

-(31.12.24) conduit Bug: https://forums.unrealengine.com/t/animstategraph-conduit-cannot-be-reentered/462978/2 (Unreal Engine Developer Forum > Character&Animation)

_________________
# Referenzquellen: 
(X = Genutzt, Y = Ungenutzt, nur in Miro, X- genutzt aber nicht in Blender) Alle zuletzt genutzt am (09.10.24)

Y Char_001: https://medium.com/@3dailyai/low-poly-character-creation-things-to-know-before-you-start-670ebc7c1b67

X Animal_001: https://dribbble.com/shots/2570767-Low-Poly-Wolf-Side#
Y Animal_002: https://poly.pizza/m/7TSeDU7o6V8
X Animal_003: https://www.turbosquid.com/de/3d-models/3d-model-ready-low-poly-goat-1358209
Y Animal_004: https://sketchfab.com/3d-models/goat-low-poly-e5f9d96f54dd4e358da2a7145b1d50b9
X Animal_005: https://lowpolyanimals.com/post/654351326869946368/chicken-from-egg-inc
Y Animal_006: https://images.app.goo.gl/fLthmQauzHkxECE88
X- Animal_007: https://www.freepik.com/premium-ai-image/3d-low-poly-horse-miniature_52698797.htm
X- Animal_008: https://cl.pinterest.com/pin/930556341732592064/

Y Esset_001: https://www.shutterstock.com/de/search/chest-low-poly
Y Esset_002: https://www.pngkey.com/detail/u2q8q8e6i1a9o0e6_by-martyisnothere-on-deviantart-low-poly-treasure-chest/
Y Esset_003: me in Paint
Y Esset_004: https://www.turbosquid.com/de/3d-models/3d-medieval-carts-pack-pbr-game-ready-2091074
X- Esset_005: https://www.turbosquid.com/de/3d-models/lowpoly-wagon-3d-1854294
Y Esset_006: https://steamcommunity.com/sharedfiles/filedetails/?id=2808075544
X- Esset_007: https://images.app.goo.gl/WZQFQkVkBeXGQyMZ7
