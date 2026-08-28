# Tiny Lena's Fishing App als PWA – Deploy-Anleitung

Der Ordner enthält alles: `index.html` (die App), `manifest.webmanifest`,
`sw.js` (Offline-Modus), `icon-192.png`, `icon-512.png`.

Einzige Voraussetzung fürs "Installieren?"-Popup: **Auslieferung über HTTPS.**

## Variante A: GitHub Pages (am schnellsten, gratis)

1. Auf github.com ein neues Repository anlegen (z.B. `fishing-app`,
   kann public oder private mit Pages sein – bei private braucht's GitHub Pro,
   also einfach public: die App enthält KEINE Daten, nur Code.
   Eure Fänge bleiben im localStorage auf dem Handy!)
2. Die 5 Dateien aus diesem Ordner hochladen (Web-Oberfläche: "Add file → Upload files")
3. Settings → Pages → Source: "Deploy from a branch" → Branch `main`, Ordner `/ (root)` → Save
4. Nach ~1 Minute läuft die App unter `https://DEINUSER.github.io/fishing-app/`
5. URL am Handy in Chrome öffnen → Chrome zeigt "Tiny Lena's Fishing App installieren?"
   (sonst: Drei-Punkte-Menü → "App installieren")

**Updates:** Neue `index.html` ins Repo hochladen (ersetzen) – beide Handys
bekommen die neue Version beim nächsten Öffnen mit Internet. Kein APK-Bau, nichts.

## Variante B: Eigenes NAS (volle Kontrolle)

Beliebiger Webserver (nginx/Web Station) der den Ordner ausliefert – ABER:
Der Install-Prompt und der Service Worker verlangen HTTPS mit gültigem Zertifikat.
Im LAN heisst das: eigene Domain + Let's Encrypt (DNS-Challenge) oder interne CA,
die auf den Handys installiert ist. Machbar, aber mehr Aufwand als Variante A.

Pragmatischer Mittelweg: GitHub Pages fürs Hosting, NAS/Filen für die Backups.

## Nach der Installation

- App-Icon auf dem Homescreen, startet im Vollbild ohne Browser-Leiste
- Android-Rücktaste navigiert in der App (History-Integration ist eingebaut)
- **Offline-fähig:** Nach dem ersten Besuch cached der Service Worker die App –
  sie startet auch am See ohne Empfang
- **Backup-Export/Teilen/Kamera funktionieren nativ** – es ist echtes Chrome
- Savina installiert von derselben URL; jede hat ihren eigenen localStorage

## Daten-Migration von der alten APK

1. Alte APK: 🧩 "Backup kopieren" (alle Teile kopieren, z.B. in eine Notiz)
2. PWA öffnen: 🧩 "Import einfügen" → Teile einfügen → Import läuft automatisch
3. In der PWA einmal "⬇️ Backup exportieren" testen – landet jetzt echt in Downloads 🎉
4. Alte APK deinstallieren

## Wichtig zu wissen

- Die App-Daten hängen am **Origin** (der URL). Solange die URL gleich bleibt,
  bleiben die Daten über alle Updates erhalten. Bei einem Hosting-Umzug:
  vorher Backup exportieren, danach importieren.
- Der Service Worker lädt Updates "Netzwerk zuerst": Mit Internet kommt immer
  die aktuelle Version, ohne Internet die zuletzt gecachte.
