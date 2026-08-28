# 🎣 Tiny Lena's Fishing App

Ein persönliches Fanglogbuch als PWA – **komplett lokal, ohne Konto, ohne Cloud, ohne Tracking.**
Alle Daten bleiben auf dem eigenen Gerät.

## Funktionen

### 🐟 Fänge
- Fänge erfassen mit Fischart, Grösse, Datum, Uhrzeit, Wetter, Technik und Köder
- Fangfoto direkt per Kamera oder aus der Galerie (wird automatisch verkleinert)
- Personal Best und letzter Fang auf dem Dashboard
- Fänge lassen sich Plätzen und Trips zuordnen

### 📍 Plätze
- Angelplätze mit Art (See, Fluss, …), Grösse und vorkommenden Fischarten
- Platzbild (z.B. Tiefenkarte) und Notizen (Schonzonen, Parkplätze, …)
- Fangübersicht pro Platz

### 🎫 Lizenzverwaltung
- Patente/Lizenzen pro Platz mit Kosten und Gültigkeit
- Automatische Warnung auf dem Dashboard, wenn eine Lizenz in den
  nächsten 14 Tagen abläuft oder bereits abgelaufen ist

### 🪱 Köder
- Softbaits und Hardbaits mit Hersteller, Farbe, Grösse und Gewicht
- Zielfisch-Tags für die schnelle Auswahl

### 🎣 Ausrüstung
- Ruten (inkl. Länge und Wurfgewicht), Rollen, Schnüre und Vorfächer
- **Tacklesets:** Rute + Rolle + Schnur + Vorfach zu fertigen Combos kombinieren

### 🧰 Terminal Tackle
- Gewichte, Haken, Jigköpfe (mit eigenem Übersichtsbild, z.B. Grössentabelle),
  Wirbel/Snaps und Sonstiges

### 🎒 Trip-Planung
- Trips mit Platz, Datum, Wetter-Notizen, Tacklesets, Ködern und Gewichten planen
- Zielfisch-Auswahl filtert die Köderliste automatisch
- **Tackle-Check:** warnt, wenn ein Köder zu schwer oder zu leicht für das
  Wurfgewicht der eingepackten Ruten ist
- Fänge direkt dem Trip zuordnen, Trips abschliessen und im Archiv nachschlagen

### 💡 Tipps & Tools
- Werkzeugliste (Kescher, Zange, …)
- Knoten-Sammlung mit Anleitungsbildern

## 💾 Daten & Backup
- Alles wird lokal im Browser-Speicher abgelegt (localStorage)
- **Backup exportieren:** kompletter Datenbestand inkl. aller Fotos als JSON-Datei
- **Backup importieren:** Datei auswählen, fertig – ideal für Gerätewechsel
  oder um den Stand auf ein zweites Handy zu übertragen

## 📲 Installation
1. Seite im Browser öffnen (GitHub Pages)
2. „App installieren" wählen (Chrome: Menü → *App installieren*)
3. Die App startet wie eine native App vom Homescreen und funktioniert
   dank Service Worker auch offline

---
*Gebaut mit einer einzigen HTML-Datei – kein Framework, kein Build, kein Backend.* 🛠
