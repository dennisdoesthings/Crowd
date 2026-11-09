# Crowd – Räumungssimulation

Einfaches Tool im Browser, um Räumungsszenarien für ein oder zwei Räume durchzuspielen und zu vergleichen.

## Starten

`index.html` im Browser öffnen. Keine Installation, läuft komplett lokal.

## Funktionen

- **Zwei Räume** nebeneinander (der zweite ist abschaltbar), Größe als Länge × Breite oder als Fläche in m² (wird dann quadratisch).
- **Türen je Wand** hinzufügen und entfernen, jeweils mit Breite, Position und offen/gesperrt. Türen in der gemeinsamen Wand verbinden die Räume, alle anderen sind Ausgänge.
- **Hindernisse** frei als Rechtecke einzeichnen, verschieben, skalieren und benennen.
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
