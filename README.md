# OffMarketDeals – Landingpage

Die öffentliche Landingpage ist unter folgender Adresse erreichbar:

**[https://johannkern.github.io/OffMarketDealsLandingpage/](https://johannkern.github.io/OffMarketDealsLandingpage/)**

## Lokal ansehen

Die Seite ist eine statische Website und benötigt weder Build-Schritt noch
zusätzliche Abhängigkeiten:

1. Öffne `index.html` direkt im Browser, zum Beispiel per Doppelklick im
   Explorer.
2. Alternativ öffne PowerShell in diesem Ordner und starte einen lokalen
   Webserver:

   ```powershell
   py -m http.server 8000
   ```

   Rufe dann <http://localhost:8000> im Browser auf. Beende den Server mit
   `Ctrl+C`.

## Seite bearbeiten und veröffentlichen

Die Quelldatei der Website ist `index.html`. Änderungen auf dem Branch `main`
werden nach dem Push automatisch über GitHub Pages veröffentlicht.

Öffne PowerShell im Repository-Ordner `landingpage` und führe nach deinen
Änderungen die folgenden Befehle aus:

```powershell
git status
git diff
git add index.html README.md
git commit -m "Landingpage aktualisieren"
git push origin main
```

Wenn du weitere Dateien bearbeitest, nimm sie ebenfalls in `git add` auf.
Nach dem Push kannst du den Build- und Veröffentlichungsstatus im
[GitHub-Actions-Bereich](https://github.com/JohannKern/OffMarketDealsLandingpage/actions)
prüfen. Bei erfolgreichem Lauf ist die aktualisierte Seite unter der oben
genannten Adresse verfügbar; es kann einen kurzen Moment dauern, bis die
Veröffentlichung sichtbar ist.

Zum Abrufen der neuesten Änderungen aus GitHub:

```powershell
git pull origin main
```

Der Push setzt eine für das Repository schreibberechtigte, bei GitHub
angemeldete Git-Identität voraus.

## Vor einer Veröffentlichung prüfen

- Die Kontaktlinks und `CONTACT_EMAIL` in `index.html` verwenden
  `johann.kern1161@gmail.com`. Passe alle Einträge an, falls sich die
  Kontaktadresse ändert.
- Ergänze ein rechtskonformes Impressum und eine individuelle
  Datenschutzerklärung und verlinke sie im Footer. Die Beschreibung auf der
  Landingpage ersetzt keine Datenschutzerklärung.
- Gleiche Aussagen zu Zugriffsschutz, Arbeitsbereichen und KI-Matching mit den
  tatsächlich verfügbaren Produkteigenschaften ab.

## Technischer Überblick

- Responsive, deutschsprachige One-Page-Website
- CSS, SVG und JavaScript sind in `index.html` enthalten; keine externen
  Bibliotheken oder Schriftarten erforderlich
- Kein Cookie-Tracking und keine Analyse-Skripte eingebaut
- Mobilmenü, FAQ und Matching-Beispiel
- Kontaktaufnahme über das E-Mail-Programm des Besuchers, kein Serverformular
- Beispielansicht und Beispielinvestor sind fiktiv gekennzeichnet

Die eigentliche OffMarketDeals-Software ist nicht Bestandteil dieser Website;
die Landingpage dient ausschließlich der Produktpräsentation.
