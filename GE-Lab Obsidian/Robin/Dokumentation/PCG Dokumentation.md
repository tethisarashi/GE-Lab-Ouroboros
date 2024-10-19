PCG Guide

Surface Sampler // Zeichnet Punkte auf Landschaft

->Points per Square Meter // Steuert die Dichte Weniger Dichte = Mehr FPS

->Point Extense // Bestimmt Größe der Punkte Überlappende Punkte werden Gefiltert

Density Filter // Filter Punkte

-> Invert // Invertiert Punkte Filter

Spacial Noise // Verteilung von Punkten durch Noise

-> Sorgt für Realistische Verteilung

Execude Blueprint // modifyer node

Scale by Density // Passt Größe von Punkten an

-> Min Wert

Min & Max Wert für scaling

-> Max Wert

Transform Points // Dreht und Verändert Punkte

-> Rotation Max auf 360° für zufällige Rotation

-> Scale Anpassbar X,Y,Z // bsp 0,75min 1,25max

-> Offset X,Y // bsp 20,20 VORSICHT MIT DIESEM WERT!

->Absolute Rotation // Sorgt dafür das bsp Bäume aufrecht bleiben

Static Mesh Spawner // Mehr meshes mehr Variation

->Mesh entries // Array füllen für Platzierte meshes

Atribute Noise // Wichtig Quelle festlegen prefix: $!