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

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-01 | Ein Computer soll sich per DDS von ROS2 zu dem Roboter verbinden können | FA | Muss | POS-A1 | TODO |
| FA-02 | **TODO: ist das requirement noch benötigt?** Der Roboter soll durch drücken der Pfeiltasten auf dem verbundenen Computer gesteuert werden können. Pfeiltaste oben: Roboter nach vorne, Pfeiltaste rechts: Roboter nach rechts drehen, Pfeiltaste runter: Roboter nach hinten, Pfeiltaste links: Roboter nach links drehen | FA | Muss | POS-A1 | TODO |
| FA-03 | Wenn auf dem verbundenen Computer die Pfeiltaste nach oben oder die Pfeiltaste nach unten gedrückt wird, bewegt sich der Roboter nach vorne oder hinten. | FA | Muss | POS-A1 | Wenn Pfeiltaste oben gedrückt wird, bewegt sich der Roboter nach vorne. Bei Pfeiltaste runter, nach hinten. Wenn beide Tasten gedrückt werden, dann soll der Roboter sich nicht bewegen. Wenn keine der zwei Tasten gedrückt wird soll er stehenbleiben. |
| FA-03 | Die Geschwindigkeit, mit der sich der Roboter gerade nach vorne oder hinten bewegt, ist 90% der einstellbaren maximalen Fahrgeschwindigkeit. | FA | Muss | POS-A1 | Wenn Pfeiltaste oben gedrückt wird, bewegt sich der Roboter nach vorne. Bei Pfeiltaste runter, nach hinten. Wenn beide Tasten gedrückt werden, dann soll der Roboter sich nicht bewegen. Wenn keine der zwei Tasten gedrückt wird soll er stehenbleiben. |
| FA-09 | Die maximale Fahrgeschwindigkeit des Roboters soll zur Laufzeit in 10% Schritten **TODO: Passt das? durch den Viewer** auf dem verbundenen Computer geändert werden können. 'W': Geschwindigkeit +10% 'S': Geschwindigkeit -10% (% ) | FA | Muss | POS-A1 | TODO |
| FA-09 | Die maximale Fahrgeschwindigkeit des Roboters soll zur Laufzeit in 10% Schritten **TODO: Passt das? durch den Viewer** auf dem verbundenen Computer geändert werden können. 'W': Geschwindigkeit +10% 'S': Geschwindigkeit -10% (% ) | FA | Muss | POS-A1 | TODO |
| FA-03 | Wenn auf dem verbundenen Computer die Pfeiltaste nach links oder die Pfeiltaste nach rechts gedrückt wird und Pfeiltaste nach vorne oder nach unten nicht gedrückt werden, dreht sich der Roboter auf der Stelle nach links oder rechts. | FA | Muss | POS-A1 | Wenn nur Pfeiltaste nach links gedrückt wird, dreht sich der Roboter auf der Stelle nach links (Linker Reifen nach Hinten, Rechter Reifen nach vorne (mit der gleichen Drehgeschwindigkeit)). Das gleiche gilt für Pfeiltaste nach rechts auch (nur halt Drehung nach rechts). Wenn Pfeiltaste nach links und rechts gleichzeitig gedrückt werden, soll der Roboter sich nicht drehen. Bei |
| FA-04 | Die Bewegungen des Roboters sollen durch drücken der Leertaste auf dem verbunden Computer gestoppt werden können. | FA | Muss | POS-A1 | TODO |
| FA-05 | Die Verbindung vom Roboter zum verbundenen Computer soll durch drücken der 'q' Taste auf diesem beendet werden können. | FA | Muss | POS-A1 | TODO |
| FA-06 | Die Tasteninputs auf dem verbundenen Computer sollen, durch ein Terminal auf diesem, an den Roboter gesendet werden sollen. | FA | Muss | POS-A1 | TODO |
| FA-07 | Die Tasteninputs im Terminal des verbundenen Computer sollen ohne drücken der Enter-Taste an den Roboter gesendet werden sollen. | FA | Muss | POS-A1 | TODO |
| FA-08 | geometry_msgs/Twist auf /cmd_vel_key mit 10 Hz veröffentlichen **TODO** | FA | Muss | POS-A1 | TODO |
| FA-10 | Die Geschwindigkeit des Roboters soll im Viewer angezeigt werden sollen **TODO** | FA | Muss | POS-A1 | TODO |
| FA-11 | Es soll auf dem Raspberry Pi des Roboters ein config.yaml Datei für einstellbare Parameter geben. | FA | Muss | POS-A1 | TODO |
| FA-12 | In config.yaml soll es einen Parameter für die Start-Geschwindigkeit geben. | FA | Muss | POS-A1 | TODO |
| FA-13 | Beim Start der Verbindung mit dem Roboter soll dieser die Parameter aus config.yaml benutzten. | FA | Muss | POS-A1 | TODO |
| FA-14 | Beim Beenden der Verbindung zum Roboter bleibt das Terminal des verbundenen Computer benutzbar. | FA | Muss | POS-A1 | TODO |
| FA-15 | **TODO: und es wird ein Stopp gesendet."** zu requirement | FA | Muss | POS-A1 | TODO |
| FA-16 | Abonniert /cmd_vel_key und /scan, veröffentlicht geometry_msgs/TwistStamped auf /cmd_vel (Typ per Parameter umschaltbar) **TODO: zu requirement** | FA | Muss | POS-A2 | TODO |
| FA-17 | In config.yaml soll die maximale linear Geschwindigkeit als Parameter eingestellt werden können | FA | Muss | POS-A2 | TODO |
| FA-18 | In config.yaml soll die maximale Winkelgeschwindigkeit als Parameter eingestellt werden können | FA | Muss | POS-A2 | TODO |
| FA-19 |  | FA | Muss | POS-A2 | TODO |
| FA-20 | TODO | FA | Muss | POS-A2 | TODO |
| FA-21 | TODO | FA | Muss | POS-A2 | TODO |
| FA-22 | TODO | FA | Muss | POS-A2 | TODO |
| FA-23 | TODO | FA | Muss | POS-A2 | TODO |
| FA-24 | TODO | FA | Muss | POS-A2 | TODO |


Movement **TODO: In Tabelle schreiben**:


Ein Computer kann sich per DDS von ROS2 zu dem Roboter verbinden.
Die Tasteninputs auf dem verbundenen Computer werden, durch ein Terminal auf diesem, an den Roboter gesendet.
Die Tasteninputs im Terminal des verbundenen Computer werden ohne drücken der Enter-Taste an den Roboter gesendet.
Die Bewegungen des Roboters sollen durch drücken der Leertaste auf dem verbunden Computer gestoppt werden können.
Die Verbindung vom Roboter zum verbundenen Computer soll durch drücken der 'q' Taste auf diesem beendet werden können.
Die Fahrgeschwindigkeit (linear velocity) des Roboters ist in Meter pro Sekunde angegeben. TODO: 
Die Fahrgeschwindigkeit des Roboters beträgt maximal 90% der maximalen Geschwindigkeit die der Roboter fahren kann.
Die Fahrgeschwindigkeit des Roboters, mit der sich der Roboter gerade nach vorne oder hinten bewegt, kann zur Laufzeit geändert werden.
Die Fahrgeschwindigkeit des Roboters kann, durch druck der Tasten 'W' und 'S' im Terminal des verbundenen Computers, eingestellt werden. 'W': +10% Geschwindigkeit 'S': -10% Geschwindigkeit.
Während im Terminal des verbundenen Computers die Pfeiltaste nach oben oder die Pfeiltaste nach unten gedrückt wird, beschleunigt der Roboter mit der Fahrgeschwindigkeit nach vorne (bei Pfeiltaste nach oben) oder hinten (bei Pfeiltaste nach unten).

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Im Terminal müssen 4 Werte angezeigt werden. Anzahl gültiger Messpunke, nächstes Objekt mit Entfernung & Winkel, kleinster Abstand je Sektor (vorne, hinten, links, rechts) und die gefahrene Strecke, die aus /odom gelesen wird. Die Werte sollten im Terminal aktualisiert werden und nicht neu ausgegeben werden. | FA | Muss | POS-A3 | Im Terminal werden die richtigen Werte ausgegeben |
| FA-XX | Ungültige Werte sollten ignoriert werden. | FA | Muss | POS-A3 | Im Terminal sollten anstatt die Ungültigen Werte, der Text "Ungültiger Wert" stehen. |

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Wenn eine Bildquelle vorhanen ist, sollte einmal pro Sekunde ein Bild gemacht werden und im Viewer angezeigt werden. | FA | Muss | POS-A4 | Im Viewer sollte jede Sekunde ein neues bild, welches von der Kamera gemacht wird, angezeigt werden. |
| FA-XX | Topic und Bildtyp sind Parameter, welche in config.yaml eingestellt werden können. | FA | Muss | POS-A4 | Nach dem ändern und speichern von den Parametern, sollten sie geupdated werden. |
| FA-XX | Mit einem Knopf im Viewer, kann das aktuelle Bild in einem ausgewählten Pfad gespeichert werden. | FA | Muss | POS-A4 | Nach dem drücken des Knopfes, erscheint das Bild im ausgewählten Pfad. |

### Teil C: Backend mit FastAPI

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


**A2 zu Requirements machen**

## Use Cases und User Stories
## Aktivitätsdiagramm
## Sequenzdiagramm
## Komponentendiagramm
## ER-Diagramm
## Ressourcenplan
## Zeitplan
