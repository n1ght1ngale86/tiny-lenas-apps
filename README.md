# 🎣 Tiny Lena's Fishing App

**Dein Tackle und Fang Kodex!**
Ein persönliches Fanglogbuch als PWA – komplett lokal, ohne Konto, ohne Cloud, ohne Tracking.
Alle Daten bleiben auf dem eigenen Gerät.

## Funktionen

### 🐟 Fänge
- Fänge erfassen mit Fischart, Grösse, Datum, Uhrzeit, Wetter, Technik und Köder
- Köderwahl zweistufig: erst Softbait/Hardbait wählen, dann übersichtliche,
  nach Hersteller sortierte Auswahl
- **Tackle-Combo:** optional festhalten, mit welchem Set (Rute/Rolle) der Fisch dran war
- Fangfoto direkt per Kamera oder aus der Galerie (wird automatisch verkleinert)
- Personal Best und letzter Fang auf dem Dashboard – letzter Fang direkt antippbar
- Fänge lassen sich Plätzen zuordnen

### 🏆 Top Gear
- Ranglisten aus den eigenen Fängen: **Top Tacklesets, Top Rigs & Techniken, Top Köder**
- Zeigt pro Eintrag Fanganzahl und grössten Fisch – was fängt viel, was fängt gross?
- Der fängigste Köder steht als Teaser direkt auf dem Dashboard

### 📍 Plätze
- Angelplätze mit Art (See, Fluss, …), Grösse und vorkommenden Fischarten
- Platzbild (z.B. Tiefenkarte) und Notizen (Schonzonen, Parkplätze, …)
- Fangübersicht pro Platz

### 🎫 Lizenzverwaltung
- Patente/Lizenzen pro Platz mit Kosten und Gültigkeit
- Automatische Warnung auf dem Dashboard, wenn eine Lizenz in den
  nächsten 14 Tagen abläuft oder bereits abgelaufen ist

### 🪱 Köder
- Softbaits und Hardbaits mit Hersteller, Grösse und Gewicht (in Gramm)
- Farbkategorien statt Farbchaos: Schockfarbe / Naturfarbe, jeweils
  Dunkel / Hell – mehrfach wählbar für Köder in mehreren Farben
- Zielfisch-Tags für die schnelle Auswahl
- **Eigenschaften fürs Feintuning:** Aktivität (aktive/passive Fische),
  Flavored (mit Aroma), geeignete Jahreszeit, geeignetes Wetter
  (Sonnig / Bewölkt) und Wassertiefe (Grund / Mittelwasser / Topwater)
- Listen automatisch A–Z nach Hersteller sortiert
- **Zielfisch-Filter:** ein Tipp auf „Barsch" zeigt nur noch Barsch-Köder
- **Köderbox teilen:** nur die Köder exportieren und auf einem anderen Gerät
  in ein bestehendes Profil dazuimportieren – Fänge & Co. bleiben unberührt,
  Duplikate werden automatisch übersprungen

### 🎣 Ausrüstung
- Ruten (inkl. Länge und Wurfgewicht), Rollen, Schnüre und Vorfächer
- **Tacklesets:** Rute + Rolle + Schnur + Vorfach zu fertigen Combos kombinieren

### 🧰 Terminal Tackle
- Gewichte, Haken, Jigköpfe (mit eigenem Übersichtsbild, z.B. Grössentabelle),
  Wirbel/Snaps und Sonstiges

### 💡 Tipps & Tools
- Werkzeugliste (Kescher, Zange, …)
- Knoten-Sammlung mit Anleitungsbildern

## 💾 Daten & Backup
- Alles wird lokal im Browser-Speicher abgelegt (localStorage)
- **Backup exportieren:** kompletter Datenbestand inkl. aller Fotos als JSON-Datei
- **Backup importieren:** Datei auswählen, fertig – ideal für Gerätewechsel
  oder um den Stand auf ein zweites Handy zu übertragen

## 📲 Installation
1. Seite im Browser öffnen (GitHub Pages -> https://n1ght1ngale86.github.io/tiny-lenas-apps/)
2. „App installieren" wählen (Chrome: Menü → *App installieren*)
3. Die App startet wie eine native App vom Homescreen und funktioniert
   dank Service Worker auch offline

## 🔮 In Planung
- **Köderberater:** schlägt anhand von Jahreszeit, Wetter, Wassertiefe, Zielfisch
  und Fischlaune den passenden Köder aus der eigenen Box vor

---
*Gebaut mit einer einzigen HTML-Datei – kein Framework, kein Build, kein Backend.* 🛠
