# 🌑 NOIR Weather Dashboard

> A luxury black-themed weather dashboard with real-time data, elegant typography, and cinematic animations — built with pure HTML, CSS, and JavaScript. No frameworks. No API key required.

![NOIR Weather](https://img.shields.io/badge/version-1.0.0-c9a96e?style=flat-square&labelColor=111111)
![License](https://img.shields.io/badge/license-MIT-c9a96e?style=flat-square&labelColor=111111)
![No API Key](https://img.shields.io/badge/API%20key-not%20required-4aaa6a?style=flat-square&labelColor=111111)
![Pure HTML](https://img.shields.io/badge/built%20with-HTML%20%2F%20CSS%20%2F%20JS-c9a96e?style=flat-square&labelColor=111111)

---

## ✨ Features

- **Real-time weather data** — current conditions updated on every search
- **5-day forecast** — daily high/low temperatures with weather icons
- **Black luxury aesthetic** — deep black background with warm gold accents and noise texture
- **Cinematic typography** — Cormorant Garamond, Cinzel, and Raleway for a high-end editorial feel
- **Animated ambient glows** — drifting gold light orbs and floating particles
- **Sun path arc** — visual tracker showing sunrise, current position, and sunset
- **Wind compass** — rotating gold needle indicating real wind direction
- **UV index, dew point, pressure, humidity, visibility** — full atmospheric data
- **°C / °F toggle** — switch units without re-fetching data
- **Fully responsive** — works on desktop and mobile
- **Zero dependencies** — no npm, no build step, no framework

---

## 📸 Preview

```
╔══════════════════════════════════════════════╗
║  NOIR WEATHER              Cuaca dalam       ║
║  ————————                  keheningan elegan ║
║                                              ║
║  [ Masukkan nama kota…  ] [°C] [°F] [ Cari ]║
║                                              ║
║  Jakarta                              ⛅     ║
║  INDONESIA                                   ║
║  31°C           Sebagian Berawan             ║
║                                              ║
║  ┌──────┬──────┬──────┬──────┐              ║
║  │ Hum  │Min/Mx│Press │Cloud │              ║
║  │  78% │27/33°│1008  │ 45%  │              ║
║  └──────┴──────┴──────┴──────┘              ║
║                                              ║
║  ☀ ─ ─ ─ ─ ─ 🌟─ ─ ─ ─ ─ ─ ─             ║
║  05:48          12:30          17:52         ║
╚══════════════════════════════════════════════╝
```

---

## 🚀 Getting Started

### Option 1 — Open directly in browser

No installation needed. Just download the file and open it.

```bash
git clone https://github.com/your-username/noir-weather.git
cd noir-weather
open weather-dashboard.html   # macOS
# or double-click the file on Windows/Linux
```

### Option 2 — Serve locally

```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .
```

Then visit `http://localhost:8000/weather-dashboard.html`

### Option 3 — Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your dashboard will be live at `https://your-username.github.io/noir-weather/weather-dashboard.html`

---

## 🔌 APIs Used

| API | Purpose | Cost |
|-----|---------|------|
| [Open-Meteo](https://open-meteo.com) | Weather data (current + forecast) | Free, no key |
| [Nominatim (OpenStreetMap)](https://nominatim.openstreetmap.org) | City geocoding (name → lat/lon) | Free, no key |

Both APIs are open and completely free. No account, no API key, no rate-limit worries for personal use.

---

## 📦 Project Structure

```
noir-weather/
│
├── weather-dashboard.html   # The entire app — single self-contained file
└── README.md
```

Everything lives in one HTML file — styles, markup, and JavaScript. No build tools, no dependencies, no configuration.

---

## 🎨 Design System

| Element | Value |
|---------|-------|
| Background | `#080808` — near-pure black |
| Surface | `#111111` — elevated cards |
| Accent | `#c9a96e` — warm gold |
| Text | `#f0ece4` — warm white |
| Display font | Cormorant Garamond (serif, italic) |
| Label font | Cinzel (Roman caps) |
| Body font | Raleway Light |
| Border | `rgba(255,255,255,0.06)` — barely-there lines |

---

## 🌍 Supported Data Points

| Data | Description |
|------|-------------|
| 🌡️ Temperature | Current, feels-like, min/max |
| 💧 Humidity | Relative humidity (%) |
| 🌬️ Wind | Speed (km/h) + direction compass |
| ⬇️ Pressure | Atmospheric pressure (hPa) |
| ☁️ Cloud cover | Sky coverage (%) |
| ☀️ UV Index | With severity label |
| 🌫️ Visibility | In km or meters |
| 🌡️ Dew Point | Dew point temperature |
| 🌅 Sun Arc | Sunrise, current position, sunset |
| 📅 5-Day Forecast | Daily high/low + condition icons |

---

## 🛠️ Customization

### Change the default city

Find this line near the bottom of the `<script>` block:

```javascript
document.getElementById('si').value = 'Jakarta';
```

Replace `'Jakarta'` with any city name.

### Change the accent color

In the `:root` CSS block, update:

```css
--gold:    #c9a96e;   /* main gold */
--gold-lt: #e8c98a;   /* light gold */
--gold-dk: #8a6a38;   /* dark gold */
```

For a cool silver tone, try `#a0a8b0`, `#c8d0d8`, `#606870`.

### Change fonts

Replace the Google Fonts import at the top with any pairing you prefer:

```html
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital@0;1&family=Jost:wght@200;300;400&display=swap" rel="stylesheet">
```

Then update the font-family references in `:root` and the relevant CSS selectors.

---

## 🌐 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile (iOS/Android) | ✅ Responsive |

---

## 📋 License

MIT License — free to use, modify, and distribute. Attribution appreciated but not required.

---

## 🙌 Acknowledgements

- Weather data by [Open-Meteo](https://open-meteo.com) — open-source weather API
- Geocoding by [Nominatim](https://nominatim.openstreetmap.org) — OpenStreetMap's geocoding service
- Fonts by [Google Fonts](https://fonts.google.com) — Cormorant Garamond, Cinzel, Raleway

---

<div align="center">
  <sub>Built with obsessive attention to detail · Dark by design · Free forever</sub>
</div>
