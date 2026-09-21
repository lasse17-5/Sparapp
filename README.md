# 🦕 Spardino – Budget-Planer & Sparziele

Eine kleine Web-App mit zwei Bereichen, die du unten per Tab wechselst:

- **Planer**: Lege pro Woche ein Budget an (Name ist mit der aktuellen Kalenderwoche vorausgefüllt, aber änderbar). Trage Ausgaben ein – der Balken füllt sich und die Farbe wechselt automatisch:
  - unter 50 % → rosa
  - 50–75 % → violett
  - 75–100 % → rot
  - über 100 % → ein weinender Dino erscheint
- **Ziele**: Erstelle "Spardinos" mit Namen und Sparziel. Trage Beiträge ein – der Dino wird passend zum Fortschritt immer weiter ausgemalt.

Alle Daten werden lokal im Browser gespeichert (`localStorage`) – es gibt keinen Server und keine Anmeldung.

## Lokal ausprobieren

Einfach `index.html` doppelklicken bzw. im Browser öffnen.

## Auf GitHub veröffentlichen (GitHub Pages)

1. Erstelle ein neues Repository auf [github.com/new](https://github.com/new), z. B. `spardino`.
2. Lade `index.html` (und diese `README.md`) in das Repository hoch – entweder per Web-Oberfläche ("Add file → Upload files") oder per Git:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Erste Version von Spardino"
   git branch -M main
   git remote add origin https://github.com/DEIN-NUTZERNAME/spardino.git
   git push -u origin main
   ```
3. Gehe im Repository auf **Settings → Pages**.
4. Wähle bei "Branch" den Branch `main` und Ordner `/ (root)`, dann **Save**.
5. Nach kurzer Zeit ist die App unter `https://DEIN-NUTZERNAME.github.io/spardino/` erreichbar.

## Datei-Struktur

```
spardino/
├── index.html   ← die komplette App (HTML, CSS, JS in einer Datei)
└── README.md
```

Da alles in einer Datei steckt, kannst du sie auch einfach anpassen: Farben, Texte und Beschriftungen findest du direkt im `<style>`- bzw. `<script>`-Block von `index.html`.
