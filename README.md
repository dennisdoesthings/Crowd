# Crowd

Einfaches Crowd-Management-Tool im Browser: Grundriss zeichnen oder als Bild hinterlegen, Durchgänge,
Hindernisse und Personenströme einstellen und die Auswirkungen in einer Simulation beobachten.

## Starten

`index.html` im Browser öffnen. Keine Installation, keine Abhängigkeiten, läuft komplett lokal.

## Funktionen

- **Karte**: Wände, Durchgänge, Hindernisse, Quellen (Start-/Zustromflächen) und Ziele zeichnen, verschieben, per Griff ändern.
- **Durchgänge**: offen/geschlossen, Einbahnregelung, Dosierung in Personen/min; Durchfluss und Zählung je Durchgang.
- **Quellen**: Startbelegung, Zustrom (P/min), Obergrenze, festes oder nächstes Ziel.
- **Crowd-Stellgrößen**: Wunschgeschwindigkeit und Streuung, Körperradius, Abstandhalten, Warn- und kritische Dichte.
- **Lagebild**: Dichte-Heatmap, maximale und Spitzendichte, Fläche über Warnschwelle, Räumungszeit, Verlauf.
- **Grundriss**: Bild (PNG/JPG/SVG) als Hintergrund laden, mit dem Werkzeug „Maßstab“ über eine bekannte Strecke kalibrieren.
- **Szenarien**: als JSON speichern/laden, automatische Zwischenspeicherung im Browser, Rückgängig (Strg+Z).

## Eigenen Grundriss verwenden

1. Unter „Karte“ das Bild laden (PDF vorher als Bild exportieren).
2. „Maßstab“ wählen, eine Strecke mit bekannter Länge nachziehen, reale Länge eingeben.
3. Wände, Durchgänge und Hindernisse über dem Plan nachzeichnen. Das Bild selbst blockiert niemanden.

Grundrisse Dritter (z. B. Veranstaltungshäuser) sind in der Regel urheberrechtlich geschützt und liegen
deshalb nicht in diesem Repository. Geladene Bilder bleiben im Browser bzw. in der exportierten JSON-Datei.

## Modell und Grenzen

Personen folgen einem Flussfeld (kürzester Weg zum Ziel) und weichen einander und Wänden über ein
vereinfachtes Social-Force-Modell aus. Das Modell ist nicht kalibriert oder validiert. Es dient der
Orientierung und dem Variantenvergleich und ersetzt kein geprüftes Sicherheits- oder Entfluchtungskonzept.
