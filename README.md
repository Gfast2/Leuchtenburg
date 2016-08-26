# Leuchtenburg

Main / Slave board firmware for Project in Museum Leuchtenburg

## Bug fix:

### 2016-3-30: 

/ Nach der Benutzung, wenn Waage inactive für mehr als 30 Sekunde nicht weiter gespielt, würde es automatisch wieder start. Vavriable ist "Waagezeit_Konstante". 

/ Bei ”Zuschwor„ Situation würde es ab sofort noch mal starten (Calibriren). Es ist c.a. 6 Schaufe Sand. 

/ Motoren von 2 bis 4 auf Motor Leistung 60% hoch eingestellt. Motor 1 auf 65% eingestellt. 

/ Sound Track Volume (1-18, Tone der Herr Böttinger) der vorne Waage auf -9 eingestellt, hintere auf -13 bleibt.

/ Waage inactive für mehr als 15 Sekunde würde es noch mal automatisch wieder start. Vavriable ist Waagezeit_Konstante

/ ? Bei ”Zu schwer„ Situation würde es ab sofort noch mal starten (Calibriren).
	
/ Pack man 6 Schaufel Sand rein. Schafft die Waage mit 40% Leistung nicht mehr.

/ Setup more power to the Motors on the vorne Waagen. Von 40% bis zu 75%. (In Main Board Code, Tab „MotorPart”). Die erste Motor von der vorne Waagen ist nicht mehr kraftvoll genug für schwere Last.

/ soundAmb(int) method (Tab „SoundRoutine”) wird auskommentiert, weil the wave trigger board immer überlastet.

/ const int Schwellwert von 200 bis zu 250 (Tab: „Main”) eingestellt, um die vierte Schale früher zu stoppen.

/ G_Max_Calib von 50 auf 100

### 2016-3-2 

/ soundAmb(int) method (Tab „SoundRoutine”) wird auskommentiert, weil the wave trigger board immer überlastet. 

/ const int Schwellwert von 200 bis zu 250 (Tab: „Main”) eingestellt, um die vierte Schale früher zu stoppen. 

/ G_Max_Calib von 50 auf 100. Das bedeutet die Waage schafft jetzt bevor überlastung noch mehr.

## TODO:

/ Wenn viel zu viel Gewicht getragt, blinkt alle lichter, aber nicht nur die ansprechende lichter, und sprecht Böttinger „Kippt alles heraus.

/ Die vierte Schale sollte beim Erfolg stelle immer automatisch zu der richtige position gehen.

/ die(int) sollte andres programmieren, dadurch wir später die Ambient Geräusche überhaupt haben dürfen.

/ Bei manche Situation, die Erfolg Höhe stimmt nicht mehr.

/ Während die Calibration Zeit, Wenn man schnell etwas neues einpacken, überlastet. Dann blinkt (nicht programmiert) die Licht, und nicht bewegt.

/ Vier Schaufe schafft die Schale, bis zu Sechs schafft es nicht mehr, und gebt die Fehler Meldung aus.

/ Erfolg Sound sollte auch die Andre Sound sperren, wenn gespielt wird.

/ Die vierte Schale sollte beim Erfolg stelle immer automatisch zu der richtige position gehen. 

/ die soundAmb(int amb) sollte andres programmieren, dadurch wir später die Ambient Geräusche haben dürfen.