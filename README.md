# Lastenheft

Projektname: Gruppe1-TurtleBot-Burger

Gruppe: Gruppe1

Namen:
- GALABURDA Alexei
- NEICOVCEN Vladislav
- REICHART Tobias
- SCHAFFER Christof

Klasse: 4AHIF

Datum: TODO

## Inhaltsverzeichnis

TODO

## Requirements

Autor: Reichart Tobias

TODO: Vlad, Alexei, Christof co-autor -> richtig anschreiben

TODO: Prio durchgehen

## A1: Steuerung

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-xx | Ein Computer kann sich per DDS von ROS2 zu dem Roboter verbinden. | FA | Muss | POS-A1 | Ein Computer kann sich mit dem Roboter verbinden |
| FA-xx | In einem Terminal in dem **keyboard_teleop** ausgeführt wird, werden alle Tasteninputs ohne das nach jedem Input Enter gedrückt werden muss, gelesen. | FA | Muss | POS-A1 | Die Tasteneingaben werden eingelesen, ohne das man danach Enter drücken muss |
| FA-xx | **keyboard_teleop** kann durch Drücken der Taste q und Strg+C beendet werden. | FA | Muss | POS-A1 | TODO |
| FA-xx | Wenn **keyboard_teleop** beendet wird, ist das Terminal wieder normal benutzbar. | FA | Muss | POS-A1 | TODO |
| FA-xx | Die Bewegungen des Roboters werden durch drücken der Leertaste auf dem verbunden Computer gestoppt. | FA | Muss | POS-A1 | TODO |
| FA-xx | Die Fahrgeschwindigkeit (linear velocity) des Roboters beträgt maximal der in **TODO: A2- linear velocity parameter linken** definierten maximalen Fahrgeschwindigkeit. | FA |Muss | POS-A1 | TODO |
| FA-xx | Die Sollgeschwindigkeit des Roboters kann im **keyboard_teleop** Terminal zur Laufzeit in 10% (% von der maximalen Geschwindigkeit die der Roboter fahren kann (0.22m/s)) Schritten geändert werden. | FA | Muss | POS-A1 | TODO |
| FA-xx | **keyboard_teleop** zeigt in der Ausgabe an, was die aktuelle **Soll**- und **Fahr**geschwindigkeit ist.| FA | Muss | POS-A1 | TODO |
| FA-xx | **keyboard_teleop** zeigt in der Ausgabe an, was die Winkelgeschwindigkeit ist.| FA | Muss | POS-A1 | TODO |
| FA-xx | Wenn im **keyboard_teleop** Terminal des verbundenen Computers die Pfeiltaste nach oben oder die Pfeiltaste nach unten gedrückt wird, wird die Fahrgeschwindigkeit (linear velocity x) auf (bei Pfeiltaste nach unten negative) **Sollgeschwindigkeit** gesetzt. | FA | Muss | POS-A1 | TODO |
| FA-xx | Wenn im **keyboard_teleop** Terminal des verbundenen Computers die Pfeiltaste nach links oder nach rechts gedrückt wird, wird die Winkelgeschwindigkeit auf (bei rechts -) 1 rad/s gesetzt. | FA | Muss | POS-A1 | TODO |
| FA-xx | Das Movement wird in **geometry_msgs/Twist** Nachrichten (lineare und angulare Velocity) mit **10 Hz** auf den Topic **/cmd_vel_key** veröffentlicht. | FA | Muss | POS-A1 | Auf dem Topic /cmd_vel_key wird in ca. 10 Hz Abständen die  |

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Im Terminal müssen 4 Werte angezeigt werden. Anzahl gültiger Messpunke, nächstes Objekt mit Entfernung & Winkel, kleinster Abstand je Sektor (vorne, hinten, links, rechts) und die gefahrene Strecke, die aus /odom gelesen wird. Die Werte sollten im Terminal aktualisiert werden und nicht neu ausgegeben werden. | FA | Muss | POS-A3 | Im Terminal werden die richtigen Werte ausgegeben |
| FA-XX | Ungültige Werte sollten ignoriert werden. | FA | Muss | POS-A3 | Im Terminal sollten anstatt die Ungültigen Werte, der Text "Ungültiger Wert" stehen. |

## A4: Kamera

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Wenn eine Bildquelle vorhanen ist, sollte einmal pro Sekunde ein Bild gemacht werden und im Viewer angezeigt werden. | FA | Muss | POS-A4 | Im Viewer sollte jede Sekunde ein neues bild, welches von der Kamera gemacht wird, angezeigt werden. |
| FA-XX | Topic und Bildtyp sind Parameter, welche in config.yaml eingestellt werden können. | FA | Muss | POS-A4 | Nach dem ändern und speichern von den Parametern, sollten sie geupdated werden. |
| FA-XX | Mit einem Knopf im Viewer, kann das aktuelle Bild in einem ausgewählten Pfad gespeichert werden. | FA | Muss | POS-A4 | Nach dem drücken des Knopfes, erscheint das Bild im ausgewählten Pfad. |

## B1: Einfache Odometrie-Kartierung

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | `/scan` und `/odom` sollen als Eingabedaten für Karte benutzt werden. | FA | Muss | POS-B1 | Wenn die Karte aus `/scan` und `/odom` gemacht wird. |
| FA-XX | Die Karte ist ein Raster und soll aus Zellen gemacht werden, deren größe einstellbar ist. | FA | Muss | POS-B1 | Die Karte wird aus einstellbaren Zellen gemacht. |
| FA-XX | Jede Zelle kann einen Wert haben. -1 steht für unbekannt, 0 steht für frei und ein wert von 1 - 100 zeigt an wie viel von der Zelle belegt ist. | FA | Muss | POS-B1 | Jede Zelle zeigt den richtigen Wert an. |
| FA-XX | Jeder gültige Messpunkt wird aus dem Roboter-Koordinatensystem in das Karten-Koordinatensystem umgerechnet. | FA | Muss | POS-B1 | Das Roboter-Koordinatensystem wird ohne Fehler in das Karten-Koordinatensystem umgerechnet. |
| FA-XX | Für die umrechnung der Koordinatensysteme, werden Position und Ausrichtung (mit der Yaw ansicht) aus der Odometrie verwendet. | FA | Muss | POS-B1 | Die Daten für die umrechnung sind die Position und Ausrichtung von der Yaw ansicht, aus der Odometrie. |
| FA-XX | Die Zelle die am Messpunkt liegt, ist eine **belegte** Zelle. Die restlichen Zellen zwischen dem Roboter und dem Messpunkt sind **frei**. | FA | Muss | POS-B1 | Nur die Zelle am Messpunkt ist eine belegte Zelle, die restlichen sind frei. |
| FA-XX | Die Karte wird durchgehen live aktualisiert. | FA | Muss | POS-B1 | Die Karte akutalisiert sich. |
| FA-XX | Die Karte kann lokal als Bild gespeichert werden. | FA | Muss | POS-B1 | Z.B. per Knopfdruck wird die Karte lokal gespeichert. (z.b. als *CoolesBild.png*) |
| FA-XX | Die Karte wird unter `/map_baseline` veröffentlicht, damit sie nicht mit `/map` von slam_toolbox kollidiert. | FA | Muss | POS-B1 | Man findet die Karte unter `/map_baseline`. |
| FA-XX | Es sollen folgende Parameter existieren, Zellgröße, Kartengröße, Kartenursprung, maximale Reichweite und Sendeintervall. | FA | Muss | POS-B1 | Die Parameter existieren und speichern die richtigen Werte. |
| FA-XX | Die aktuelle Karte wird entweder periodisch oder per Anfrage, durch den `map_uploader`, ans Backend gesendet. | FA | Muss | POS-B1 | Das Backend kriegt die aktuelle Karte. |

**TODO:** Hinweise zur Umsetzung aufschreiben.

### C: Backend mit FastAPI

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-C01 | Das Backend muss über `POST /maps` eine neue Karte im JSON-Format entgegennehmen und speichern. | FA | Muss | POS-C | Eine gültige Anfrage liefert den Statuscode 201 und die ID der neuen Karte. Die Karte ist danach über `GET /maps/{id}` abrufbar. |
| FA-C02 | Das Backend muss über `GET /maps` eine Liste aller gespeicherten Karten ohne Rasterdaten liefern. | FA | Muss | POS-C | Die Antwort hat den Statuscode 200 und enthält alle gespeicherten Karten mit ihren Metadaten. Kein Eintrag enthält Rasterdaten. Ohne gespeicherte Karten ist die Liste leer. |
| FA-C03 | Das Backend muss über `GET /maps/{id}` genau eine Karte mit allen Metadaten und Rasterdaten liefern. | FA | Muss | POS-C | Die Antwort hat den Statuscode 200. Metadaten und Rasterdaten stimmen mit den gespeicherten Daten überein. |
| FA-C04 | Das Backend muss über `DELETE /maps/{id}` eine gespeicherte Karte löschen. | FA | Muss | POS-C | Die Antwort hat den Statuscode 204. Ein anschließendes `GET /maps/{id}` liefert 404 und die Karte fehlt in `GET /maps`. |
| FA-C05 | Das Backend muss über `GET /health` seinen Status liefern. | FA | Muss | POS-C | Bei laufendem Backend hat die Antwort den Statuscode 200 und enthält ein Statusfeld (z. B. `{"status": "ok"}`). |
| FA-C06 | Eine Karte muss mindestens aus folgenden Feldern bestehen: ID, Name, Erstellungszeitpunkt, Quelle (`odometry_baseline` oder `slam_toolbox`), Frame, Zellgröße, Breite, Höhe, Ursprung (x, y, yaw) und Rasterdaten. | FA | Muss | POS-C | Die Antwort von `GET /maps/{id}` enthält jedes dieser Felder. |
| FA-C07 | Das Backend muss die ID einer neuen Karte selbst vergeben. | FA | Muss | POS-C | Zwei nacheinander gespeicherte Karten haben unterschiedliche IDs. Eine in der Anfrage mitgeschickte ID wird nicht übernommen. |
| FA-C08 | Das Backend muss alle Eingaben mit Pydantic-Modellen validieren und fehlerhafte Daten ablehnen. | FA | Muss | POS-C | Eine Anfrage mit fehlendem Pflichtfeld oder falschem Datentyp liefert den Statuscode 422. Es wird keine Karte gespeichert. |
| FA-C09 | Das Backend muss prüfen, ob die Rasterdaten zur Kartengröße passen: Die Anzahl der Zellen muss Breite × Höhe entsprechen und jede Zelle muss den Wert -1 oder einen Wert von 0 bis 100 haben. | FA | Soll | POS-C | Eine Anfrage mit falscher Zellenanzahl oder einem Wert außerhalb des Bereichs liefert den Statuscode 422. |
| FA-C10 | Das Backend muss bei Zugriff auf eine nicht vorhandene Karten-ID einen Fehler melden. | FA | Muss | POS-C | `GET /maps/{id}` und `DELETE /maps/{id}` mit einer unbekannten ID liefern den Statuscode 404. |
| FA-C11 | Das Backend muss die Karten in einer Datenbank (SQLite) dauerhaft speichern. | FA | Muss | POS-C | Nach einem Neustart des Backends liefert `GET /maps` dieselben Karten wie vor dem Neustart. |
| FA-C12 | Die schreibenden Endpunkte (`POST /maps`, `DELETE /maps/{id}`) müssen durch einen API-Schlüssel im HTTP-Header geschützt sein. | FA | Muss | POS-C | Eine Anfrage ohne oder mit falschem Schlüssel liefert den Statuscode 401 und ändert keine Daten. Mit richtigem Schlüssel wird die Anfrage ausgeführt. Lesende Endpunkte funktionieren ohne Schlüssel. |
| FA-C13 | Der API-Schlüssel muss über eine Umgebungsvariable oder eine nicht eingecheckte Datei konfiguriert werden. | FA | Muss | POS-C | Im Repository steht kein Schlüssel, nur eine Vorlage (`.env.example`). Nach dem Ändern der Umgebungsvariable und einem Neustart gilt der neue Schlüssel. |
| FA-C14 | Das Backend muss eine automatisch erzeugte API-Dokumentation unter `/docs` bereitstellen. | FA | Muss | POS-C | `/docs` ist im Browser erreichbar und zeigt alle fünf Endpunkte. |
| NFA-C01 | Das Backend muss in einem eigenen GitHub-Repository liegen und auf jedem Rechner mit Python ohne ROS startbar sein. | NFA | Muss | POS-C | Auf einem Rechner ohne ROS-Installation startet das Backend nach der Anleitung in der README und `GET /health` liefert 200. |
| NFA-C02 | Das Backend muss automatisierte Tests mit pytest und dem FastAPI-Testclient haben. | NFA | Muss | POS-C | `pytest` läuft ohne Fehler durch. Es gibt mindestens einen Test pro Endpunkt und je einen Test für die Fehlerfälle 401, 404 und 422. |
| NFA-C03 | Das Datenformat einer Karte muss in der README dokumentiert sein. | NFA | Muss | POS-C | Die README enthält je eine Beispiel-Anfrage und eine Beispiel-Antwort für `POST /maps`. |
|||||||
|||||||
| FA-U01 | Der Node `map_uploader` muss die ausgewählte Kartenaufnahme (Baseline oder SLAM) per HTTP-Anfrage `POST /maps` an das Backend senden. | FA | Muss | POS-C | Nach dem Auslösen einer Aufnahme erscheint die Karte mit der richtigen Quelle in `GET /maps`. |
| FA-U02 | Die Backend-Adresse und der API-Schlüssel müssen Parameter des Nodes `map_uploader` sein. | FA | Muss | POS-C | Nach dem Ändern der Backend-Adresse in der Parameterdatei und einem Neustart des Nodes sendet er an die neue Adresse. Der Schlüssel steht nicht im Repository. |
| FA-U03 | Wenn das Backend nicht erreichbar ist, darf der Node `map_uploader` nicht abstürzen. Er muss den Fehler melden und das Senden später erneut versuchen. | FA | Muss | POS-C | Bei gestopptem Backend läuft der Node weiter und gibt eine Fehlermeldung im Log aus. Nach dem Start des Backends wird die Karte ohne Neustart des Nodes übertragen. |

## D: Viewer
| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Der Viewer muss in einem eigenen Repository sein und ohne ROS funktionsfähig sein. | FA | Muss | POS-D| Der Viewer funktioniert auch ohne ROS. |
| FA-XX | Der Viewer ruft eine Liste von Karten beim Backend ab und zeigt diese an. | FA | Muss | POS-D| Die Kartenliste wird vom Backend abgerufen und im Viewer angezeigt. |
| FA-XX | Das Raster einer Karte wird grafisch angezeigt und die verschiedenen Zellenarten werden farbisch angezeigt. *(Siehe B1 **TODO: Genaue Aufgabe hinschreiben** *) | FA | Muss | POS-D| Verschieden Zellen (unbekannt, frei und belegt) haben unterschiedliche Farben. |
| FA-XX | Jede Karte hat verschiedene Parameter, die auch angezeigt werden. Name, Erstellungszeit, Zellgröße und Größe der Karte. | FA | Muss | POS-D| Die verschiedenen Parameter werden im Viewer für jede Karte angezeigt. |
| FA-XX | Per Schaltfläche oder Taste wird die Liste der Karten aktualisiert. | FA | Muss | POS-D| Nach dem input wird die Liste erneuert. |
| FA-XX | Fehlermeldungen die passieren können, wenn das Backend nicht erreicht werden kann, sollen verständlich sein. | FA | Muss | POS-D| Fehlermeldungen die auftauchen sollen leicht verstanden werden können. |
| FA-XX | Die Technologie für den Viewer ist frei wählbar, soll aber im README.md begründet werden. | FA | Muss | POS-D| Im README.md steht der grund warum wir die Technologie gewählt haben, welche wir haben. |
## Use Cases und User Stories
## Aktivitätsdiagramm
## Sequenzdiagramm
## Komponentendiagramm
## ER-Diagramm
## Ressourcenplan
## Zeitplan
