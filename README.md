# Crowd – Räumungssimulation

Einfaches Tool im Browser, um Räumungsszenarien für ein oder zwei Räume durchzuspielen und zu vergleichen.

## Starten

`index.html` im Browser öffnen. Keine Installation, läuft komplett lokal.

## Funktionen

- **Zwei Räume** nebeneinander (der zweite ist abschaltbar), Größe als Länge × Breite oder als Fläche in m² (wird dann quadratisch).
- **Türen je Wand** hinzufügen und entfernen, jeweils mit Breite, Abstand in Metern ab der West- bzw. Nordecke und offen/gesperrt. Die Karte zeigt die Wandstücke zwischen Ecken und Türen mit Maß. Türen in der gemeinsamen Wand verbinden die Räume, alle anderen sind Ausgänge.
- **Hindernisse** einzeichnen oder über die Liste anlegen, dort Breite, Tiefe und Position in Metern eingeben und wieder entfernen.
- **Ausweichen bei Stau**: einstellbarer Anteil der Personen wählt einen anderen Weg, sobald die Dichte auf dem kürzesten Weg eine Schwelle überschreitet.
- **Bestuhlung**: Blöcke nebeneinander und hintereinander, Reihen pro Block, Stühle pro Reihe, Gangbreite, Belegung in %.
- **Stehende Personen** je Raum zusätzlich zur Bestuhlung.
- **Lagebild**: Räumungszeit, Dichte-Heatmap, Spitzendichte, Personen ohne erreichbaren Ausgang.
- **Szenarien** benennen, speichern, laden, als Datei exportieren/importieren. Jeder vollständige Durchlauf landet in der Vergleichstabelle.
- Tür in der Karte anklicken: Einbahnregelung und Dosierung (Personen/min).

## Modell und Grenzen

Personen laufen auf dem kürzesten Weg zum nächsten Ausgang und weichen einander und Wänden aus
(vereinfachtes Social-Force-Modell, Stuhl 0,5 m breit, Reihenabstand 1,0 m). Keine Reaktionszeit, alle
starten gleichzeitig. Das Modell ist nicht kalibriert oder validiert: Es eignet sich zum Veranschaulichen
und zum Vergleich von Varianten, nicht als Nachweis für ein Sicherheits- oder Entfluchtungskonzept.
