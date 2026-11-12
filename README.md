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

TODO: Vlad co-autor -> richtig anschreiben

TODO: Prio durchgehen

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-01 | Ein Computer soll sich per DDS von ROS2 zu dem Roboter verbinden können | FA | Muss | POS-A1 | TODO |
| FA-02 | Der Roboter soll durch drücken der Pfeiltasten auf dem verbundenen Computer gesteuert werden können. Pfeiltaste oben: Roboter nach vorne, Pfeiltaste rechts: Roboter nach rechts drehen, Pfeiltaste runter: Roboter nach hinten, Pfeiltaste links: Roboter nach links drehen | FA | Muss | POS-A1 | TODO |
| FA-03 | Wenn eine Fahrtaste (Pfeiltaste oben & runter) und eine Drehtaste (Pfeiltaste links & rechts) gleichzeitig gedrückt werden, fahrt der Roboter in einem Bogen. | FA | Muss | POS-A1 | Wenn Pfeiltaste vorne und Pfeiltaste links gedrückt werden, wird der rechte Reifen schneller, also fahrt der Roboter nach vorne links in einem Bogen. Das Gleiche auch mit den anderen Tasten. |
| FA-04 | Die Bewegungen des Roboters sollen durch drücken der Leertaste auf dem verbunden Computer gestoppt werden können. | FA | Muss | POS-A1 | TODO |
| FA-05 | Die Verbindung vom Roboter zum verbundenen Computer soll durch drücken der 'q' Taste auf diesem beendet werden können. | FA | Muss | POS-A1 | TODO |
| FA-06 | Die Tasteninputs auf dem verbundenen Computer sollen, durch ein Terminal auf diesem, an den Roboter gesendet werden sollen. | FA | Muss | POS-A1 | TODO |
| FA-07 | Die Tasteninputs im Terminal des verbundenen Computer sollen ohne drücken der Enter-Taste an den Roboter gesendet werden sollen. | FA | Muss | POS-A1 | TODO |
| FA-08 | geometry_msgs/Twist auf /cmd_vel_key mit 10 Hz veröffentlichen **TODO** | FA | Muss | POS-A1 | TODO |
| FA-09 | Die Geschwindigkeit des Roboters soll zur Laufzeit in 10% Schritten durch den Viewer auf dem verbundenen Computer geändert werden können. 'W': Geschwindigkeit +10% 'S': Geschwindigkeit -10% | FA | Muss | POS-A1 | TODO |
| FA-10 | Die Geschwindigkeit des Roboters soll im Viewer angezeigt werden sollen **TODO** | FA | Muss | POS-A1 | TODO |
| FA-11 | Es soll auf dem Raspberry Pi des Roboters ein config.yaml Datei für einstellbare Parameter geben. | FA | Muss | POS-A1 | TODO |
| FA-12 | In config.yaml soll es einen Parameter für die Start-Geschwindigkeit geben. | FA | Muss | POS-A1 | TODO |
| FA-13 | Beim Start der Verbindung mit dem Roboter soll dieser die Parameter aus config.yaml benutzten. | FA | Muss | POS-A1 | TODO |
| FA-14 | Beim Beenden der Verbindung zum Roboter bleibt das Terminal des verbundenen Computer benutzbar. | FA | Muss | POS-A1 | TODO |
| FA-15 | **TODO: und es wird ein Stopp gesendet."** zu requirement | FA | Muss | POS-A1 | TODO |

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Im Terminal müssen 4 Werte angezeigt werden. Anzahl gültiger Messpunke, nächstes Objekt mit Entfernung & Winkel, kleinster Abstand je Sektor (vorne, hinten, links, rechts) und die gefahrene Strecke, die aus /odom gelesen wird. Die Werte sollten im Terminal aktualisiert werden und nicht neu ausgegeben werden. | FA | Muss | POS-A3 | Im Terminal werden die richtigen Werte ausgegeben |
| FA-XX | Ungültige Werte sollten ignoriert werden. | FA | Muss | POS-A3 | Im Terminal sollten anstatt die Ungültigen Werte, der Text "Ungültiger Wert" stehen. |

| ID | Anforderung | Typ | Priorität | Quelle | Abnahmekriterium |
|-|-|-|-|-|-|
| FA-XX | Wenn eine Bildquelle vorhanen ist, sollte einmal pro Sekunde ein Bild gemacht werden und im Viewer angezeigt werden. | FA | Muss | POS-A4 | Im Viewer sollte jede Sekunde ein neues bild, welches von der Kamera gemacht wird, angezeigt werden. |
| FA-XX | Topic und Bildtyp sind Parameter, welche in config.yaml eingestellt werden können. | FA | Muss | POS-A4 | Nach dem ändern und speichern von den Parametern, sollten sie geupdated werden. |
| FA-XX | Mit einem Knopf im Viewer, kann das aktuelle Bild in einem ausgewählten Pfad gespeichert werden. | FA | Muss | POS-A4 | Nach dem drücken des Knopfes, erscheint das Bild im ausgewählten Pfad. |


**A2 zu Requirements machen**

## Use Cases und User Stories
## Aktivitätsdiagramm
## Sequenzdiagramm
## Komponentendiagramm
## ER-Diagramm
## Ressourcenplan
## Zeitplan
