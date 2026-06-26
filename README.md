<div align="center">

<img src="assets/logo.png" width="240" alt="SelfPoolTracker logo" />


**Pool water-quality tracker that runs entirely in your browser — pH, chlorine, redox & temperature logging with traffic-light status and dosing recommendations. No server, no cloud, no account.**

![Type](https://img.shields.io/badge/type-browser%20app-33A78C)
![Version](https://img.shields.io/badge/version-1.0.2-33A78C)
![License](https://img.shields.io/badge/license-MIT-8A9CAA)
![Stack](https://img.shields.io/badge/stack-single--file%20HTML-43D3AD)
![Storage](https://img.shields.io/badge/storage-local%20file%20%2F%20localStorage-9DBDD0)

[English](#english) · [Deutsch](#deutsch)

</div>

---

## English

SelfPoolTracker is a single-file web app for keeping your pool chemistry in check. Open one HTML file in Chrome or Edge, enter your pool dimensions, and log your measurements. Every value gets an automatic green / yellow / red status and a concrete dosing recommendation based on your pool volume. Data is stored locally — either in a JSON file on your own computer (File System Access API) or in the browser's `localStorage`. Nothing ever leaves your device.

### Features

- **Pool volume calculator** — Oval, Round and Rectangular pools with automatic shape-based labels
- **Daily measurement log** — pH, free chlorine, redox (mV), temperature, date & time
- **Automatic status** — green / yellow / red traffic light for every value
- **Dosing recommendations** — pH-Minus, pH-Plus and quick-chlorine amounts calculated from your pool volume
- **Dosing calculator** — standalone calculator for any manual adjustment, incl. shock chlorination
- **File-based storage** — data saved to a local JSON file (no cloud, no cache loss) with `localStorage` fallback
- **CSV export** — export your full measurement history
- **DE / EN** — German and English UI, switchable at runtime
- **Self brand** — dark theme, teal accent, Exo 2 + IBM Plex Mono

### Usage

1. Open `index.html` in **Chrome** or **Edge** (the File System Access API is required for file storage)
2. Set your pool dimensions → volume is calculated automatically
3. Click **"📂 Datei öffnen / neu erstellen"** to link a data file on your computer
4. Enter measurements — data saves automatically after each entry

> Firefox does not support the File System Access API. There it falls back to `localStorage`, so use Chrome or Edge for file-based storage.

### Ideal values

| Parameter | Min | Ideal | Max | Unit |
|-----------|-----|-------|-----|------|
| pH | 7.2 | 7.2 – 7.6 | 7.6 | – |
| Free chlorine | 0.5 | 0.5 – 1.5 | 1.5 | mg/l |
| Redox / MV | 650 | 650 – 750 | 750 | mV |
| Temperature | 15 | 20 – 28 | 35 | °C |

---

## Deutsch

SelfPoolTracker ist eine Single-File-Webapp, mit der du deine Poolwerte im Griff behältst. Eine HTML-Datei in Chrome oder Edge öffnen, Pool-Maße eintragen und Messwerte loggen. Jeder Wert bekommt automatisch einen grün / gelb / rot-Status und eine konkrete Dosierempfehlung anhand deines Pool-Volumens. Die Daten liegen lokal — entweder in einer JSON-Datei auf deinem Rechner (File System Access API) oder im `localStorage` des Browsers. Es verlässt nichts dein Gerät.

### Funktionen

- **Pool-Volumenrechner** — Oval, Rund und Rechteckig mit automatischen, formabhängigen Bezeichnungen
- **Tägliches Mess-Log** — pH, freies Chlor, Redox (mV), Temperatur, Datum & Uhrzeit
- **Automatischer Status** — grün / gelb / rot-Ampel für jeden Wert
- **Dosierempfehlungen** — pH-Minus, pH-Plus und Schnellchlor-Mengen aus dem Pool-Volumen berechnet
- **Dosierungsrechner** — eigenständiger Rechner für jede manuelle Anpassung, inkl. Schockchlorung
- **Dateibasierte Speicherung** — Daten in einer lokalen JSON-Datei (keine Cloud, kein Cache-Verlust) mit `localStorage`-Fallback
- **CSV-Export** — kompletter Messverlauf als CSV
- **DE / EN** — deutsche und englische Oberfläche, zur Laufzeit umschaltbar
- **Self-Brand** — Dark-Theme, Teal-Akzent, Exo 2 + IBM Plex Mono

### Benutzung

1. `index.html` in **Chrome** oder **Edge** öffnen (File System Access API für Datei-Speicherung nötig)
2. Pool-Maße setzen → Volumen wird automatisch berechnet
3. Auf **"📂 Datei öffnen / neu erstellen"** klicken, um eine Datendatei auf dem Rechner zu verknüpfen
4. Messwerte eintragen — speichert nach jedem Eintrag automatisch

> Firefox unterstützt die File System Access API nicht. Dort greift der `localStorage`-Fallback — für Datei-Speicherung Chrome oder Edge nutzen.

---

## Project structure

```
selfpooltracker/
├── index.html        # Single-file app (UI + logic + i18n)
├── assets/
│   └── logo.png      # Branded SelfPoolTracker wordmark
├── logo/
│   └── shield.png    # Self shield emblem (in-app header)
└── README.md
```

## Brand

Uses the **Self Design System** — tokens, fonts and shield from [`brand-kit`](../brand-kit/).

- Colors: `--self-teal` `#33a78c` · `--self-bg-0` `#080c11`
- Fonts: Exo 2 · IBM Plex Mono

## License

MIT © Self Projects
