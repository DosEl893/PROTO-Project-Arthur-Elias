# PROTO-Project-Arthur-Elias
Project PROTO2 Arthur &amp; Elias


Creative/Survival

Der Node-RED-Flow ist mit einem Taster am Digilab (PIN 40) verbunden. Wenn der Knopf gedrückt wird, wird das Signal an einen Umschaltknoten weitergeleitet. Dieser wechselt zwischen zwei Zuständen (Creative/Survival) und setzt jeweils einen anderen Wert in msg.payload. Anschließend wird eine Datei (rcon) ausgeführt, die über RCON einen Befehl an den Minecraft-Server sendet.
Dadurch kann durch eine Taste der Spielmodus des Minecraft-Servers zwischen Creative und Survival umgeschaltet werden.

Day/Night

Der Node-RED-Flow ist mit zwei Taster am Digilab (PIN 35,PIN 36) verbunden. Jeder Taster ist für eine bestimmte Tageszeit auf dem Minecraft-Server zuständig: Ein Knopf setzt die Zeit auf Tag, der andere auf Nacht. Beim Drücken eines Knopfes wird den entsprechender Wert in msg.payload gespeichert und an den RCON-Knoten weitergegeben. Dieser sendet den passenden Befehl an den Minecraft-Server, sodass die Spielzeit direkt auf Tag oder Nacht geändert wird.

Online Spieler in LCD


Music

Leben des Spielers in Led
