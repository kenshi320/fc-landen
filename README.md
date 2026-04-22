# FC Landen — Trainingsplanning PWA

Een Progressive Web App voor het beheren van trainingsplanning, terreinverdeling en kleedkamers voor FC Landen.

## 🚀 Live app

Na het instellen van GitHub Pages is de app beschikbaar op:
`https://<jouw-gebruikersnaam>.github.io/fc-landen/`

## 📱 Installeren als app

1. Open de link in Chrome (Android) of Safari (iPhone)
2. Tik op **"Installeren"** in de banner, of via het menu → "Toevoegen aan beginscherm"
3. De app werkt daarna ook **offline**

## ✨ Functies

- **Teams** — overzicht per ploeg met trainingsschema
- **Kalender** — weekoverzicht in twee blokken (vroeg 18:00–19:15 / laat 19:30–21:00)
- **Terreinen** — bezettingsgraad per terrein (Kunstgras, B-veld, C-veld)
- **Kleedkamers** — automatische verdeling van 6 kleedkamers per dag/blok
- **Overzicht** — terreinstatistieken per ploeg + bezettingsgrafiek
- **Offline werking** via Service Worker
- **Automatisch opslaan** van wijzigingen in de browser

## 🏗️ Deployment instellen

1. **Fork of push** dit project naar een GitHub repository
2. Ga naar **Settings → Pages**
3. Onder **Source**: kies **GitHub Actions**
4. Push naar `main` → de app wordt automatisch gedeployed

## 📁 Projectstructuur

```
fc-landen/
├── index.html          # Volledige PWA app (één bestand)
├── manifest.json       # PWA manifest (naam, iconen, kleuren)
├── sw.js               # Service Worker (offline caching)
├── icons/
│   ├── icon-192.png    # App icoon (klein)
│   └── icon-512.png    # App icoon (groot)
└── .github/
    └── workflows/
        └── deploy.yml  # Automatische deployment naar GitHub Pages
```

## 🛠️ Lokaal testen

```bash
# Simpele lokale server (Python)
python3 -m http.server 8080

# Of met Node.js
npx serve .
```

Open dan `http://localhost:8080` in je browser.

> ⚠️ Service Workers werken alleen op HTTPS of localhost — test dus lokaal of via GitHub Pages.
