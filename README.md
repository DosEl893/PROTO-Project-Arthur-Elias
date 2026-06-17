# PROTO-Project-Arthur-Elias
Project PROTO2 Elias &amp; Arthur


Creative/Survival

Der Node-RED-Flow ist mit einem Taster am Digilab (PIN 40) verbunden. Wenn der Knopf gedrückt wird, wird das Signal an einen Umschaltknoten weitergeleitet. Dieser wechselt zwischen zwei Zuständen (Creative/Survival) und setzt jeweils einen anderen Wert in msg.payload. Anschließend wird eine Datei (rcon) ausgeführt, die über RCON einen Befehl an den Minecraft-Server sendet.
Dadurch kann durch eine Taste der Spielmodus des Minecraft-Servers zwischen Creative und Survival umgeschaltet werden.

Day/Night

Der Node-RED-Flow ist mit zwei Taster am Digilab (PIN 35,PIN 36) verbunden. Jeder Taster ist für eine bestimmte Tageszeit auf dem Minecraft-Server zuständig: Ein Knopf setzt die Zeit auf Tag, der andere auf Nacht. Beim Drücken eines Knopfes wird den entsprechender Wert in msg.payload gespeichert und an den RCON-Knoten weitergegeben. Dieser sendet den passenden Befehl an den Minecraft-Server, sodass die Spielzeit direkt auf Tag oder Nacht geändert wird.

Online Spieler in LCD

Der dargestellte Node-RED-Flow ermöglicht die Anzeige der aktuellen Spieleranzahl auf dem Minecraft-Server. Wird ein Knopf gedrückt, sendet der Flow eine Anfrage an den Server. Die erhaltenen Informationen werden in msg.payload gespeichert und anschließend von einer Funktion verarbeitet. Das Ergebnis wird auf einem Display des Raspberry Pi ausgegeben. So kann jederzeit angezeigt werden, wie viele Spieler aktuell auf dem Server online sind.

Leben des Spielers in Led

Der dargestellte Node-RED-Flow ermöglicht die Anzeige der aktuellen Lebenspunkte (Herzen) eines Spielers auf dem Minecraft-Server. Wird ein Knopf am Digilab gedrückt, werden die Spielerinformationen vom Server abgerufen. Eine Funktion verarbeitet anschließend die Anzahl der verbleibenden Herzen und steuert mehrere LEDs an. Jede LED repräsentiert einen bestimmten Gesundheitszustand des Spielers. Je nach Anzahl der Herzen werden die entsprechenden LEDs ein- oder ausgeschaltet, sodass der aktuelle Lebensstatus des Spielers direkt über die LED-Anzeige sichtbar wird.
