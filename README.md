# FC Landen — Trainingsplanning PWA

Progressive Web App voor trainingsplanning, terreinbeheer en kleedkamerverdeling van FC Landen.

## Live app
`https://<jouw-gebruikersnaam>.github.io/fc-landen/`

## Installeren als app
1. Open de link in Chrome (Android) of Safari (iPhone)
2. Tik op **"Installeren"** of via menu → "Toevoegen aan beginscherm"

## Functies
- **Teams** — trainingsschema per ploeg, trainingen toevoegen/verwijderen
- **Kalender** — weekoverzicht met drag & drop (dag én blok wisselen, terrein kiezen)
- **Terreinen** — bezettingsgraad per terrein
- **Kleedkamers** — automatische verdeling + drag & drop om te wisselen
- **Overzicht** — statistieken + bezettingsgrafiek
- Offline werking, automatisch opslaan

## GitHub Pages instellen
1. Push naar een **public** repository
2. Settings → Pages → Source: **GitHub Actions**
3. Na de eerste push is de app live

## Lokaal testen
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Bestanden
```
fc-landen/
├── index.html          # Volledige app
├── manifest.json       # PWA manifest
├── sw.js               # Service Worker (offline)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── .github/workflows/
    └── deploy.yml      # Auto-deployment
```
