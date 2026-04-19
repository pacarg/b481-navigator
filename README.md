# B481 Streckennavigator — Emsdetten / Greven

A lightweight, single-file web app built for the local community around the **B481 roadworks (2026)** between Emsdetten and Greven, NRW.

No installation needed. Opens directly in any mobile browser.

🔗 **[Open the app](https://pacarg.github.io/b481-navigator/)**

---

## What it does

- Automatically detects the current construction phase based on today's date
- Displays a color-coded alert (green / amber / red) for the active road status
- Suggests the official detour via Saerbeck (B219 → B475) when the B481 is closed
- Adds the detour as a waypoint when opening Google Maps, so you don't get routed through the closed section
- Supports GPS auto-location or manual address input as starting point
- Allows planning multiple destinations in a single route
- Works in **German 🇩🇪 / English 🇬🇧 / Spanish 🇪🇸**

---

## Why this exists

Google Maps and Waze update their road closure data with delays. This app has the B481 construction schedule built in and warns you **before you leave**, not after you're already on the road.

---

## Construction phases (B481 Emsdetten–Greven)

| Phase | Period | Status |
|-------|--------|--------|
| Phase 1 | ~July 2026 — ~Sept 2026 | Full closure (both directions) |
| Phase 2 | ~Sept 2026 — ~Mar 2027 | One-way towards Emsdetten only |
| Complete | After ~Mar 2027 | New 2+1 road operational |

> Exact dates to be confirmed by Straßen.NRW after contract award (spring 2026).
> Official project page: [Straßen.NRW B481](https://www.strassen.nrw.de/de/b481-ersatzneubau-von-drei-bauwerken-und-fahrbahnsanierung-zwischen-greven-und-emsdetten-projektueberblick.html)

---

## Updating construction dates

The app includes a password-protected admin panel (⚙ icon in the header) to update the phase dates without editing code. Changes are saved locally in the browser via `localStorage`.

---

## Tech stack

- Single HTML file — no framework, no dependencies, no build step
- Vanilla JavaScript
- Google Maps URL API (no API key required)
- Nominatim / OpenStreetMap for reverse geocoding
- Deployable on any static host (GitHub Pages, Hostinger, Netlify, etc.)

---

## Map data

Road map © [Straßen.NRW](https://www.strassen.nrw.de) — used for reference purposes.

---

*Built by [Pablo Churín](https://guiatecnologico.com) as a free community tool for Emsdetten, Deutschland.*
