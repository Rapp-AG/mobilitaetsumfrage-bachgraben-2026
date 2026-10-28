# Mobilitätsumfrage Bachgraben 2026

Statische Landingpage (GitHub Pages) mit QR-Code zur Online-Umfrage und drei Downloads.

## Struktur

```
docs/
  index.html               Seite
  .nojekyll                Jekyll-Verarbeitung deaktiviert
  assets/css/style.css     Styles
  assets/img/              Logo und QR-Code
  downloads/               Excel-Vorlage, Word-Fragebogen, PDF Ergebnisse 2021
```

## Vor dem Veröffentlichen anpassen

1. In `docs/index.html` `SURVEY_LINK_HERE` durch die Umfrage-URL ersetzen.
2. `docs/assets/img/qr-umfrage.svg` durch den QR-Code zur Umfrage-URL ersetzen (gleicher Dateiname; bei PNG den Pfad in `index.html` anpassen).
3. Die drei Dokumente in `docs/downloads/` ablegen (Dateinamen siehe dortige README).

## Lokal ansehen

```powershell
python -m http.server 8000 --directory docs
```

Danach http://localhost:8000 öffnen.

## Veröffentlichen mit GitHub Pages

Repository auf GitHub pushen, dann unter **Settings > Pages**: Source `Deploy from a branch`, Branch `main`, Ordner `/docs`.