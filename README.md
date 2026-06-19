# TKGM Field Command Center

A live operations **command center** for **Tulluu Kaapi Gold Mine (TKGM S.C.)** — the desktop control-room counterpart to the TKGM field-safety mobile app. Dispatchers monitor field personnel in real time across the Tulu Kapi concession (Gambella / West Wollega, Ethiopia).

Single self-contained `index.html` — no build step. Just open it in a browser.

## Features

- **Live Map** — OpenStreetMap (Leaflet + CARTO Voyager tiles) with the concession boundary, restricted-pit geofence, base camp, and personnel markers that drift, pulse, and trail in real time.
- **Personnel** — roster data table with status, battery, signal, last check-in, and live coordinates.
- **Incidents** — severity board (critical / warning / info) with status tracking.
- **Geofences** — defined zones (boundary, exclusion, safe zone, work zone, corridor) with live occupancy.
- **Reports** — operational KPIs, a 7-day check-ins chart, and generated-report list.
- **Comms Log** — dispatch ↔ field radio transcript with a working broadcast composer.
- **SOS handling** — a distress scenario triggers a live alert banner, map fly-to, and acknowledge/dispatch flow.

## Design

- **Theme:** light command-center, drawn from the TKGM brand (charcoal slate + gold `#d98a0b`).
- **Type system:** [Geist + Geist Mono](https://vercel.com/font) (Vercel) — built for technical, data-dense interfaces.
- **Stack:** plain HTML / CSS / JS + [Leaflet](https://leafletjs.com/). All demo data lives in arrays at the top of the `<script>` in `index.html`, ready to wire to a real feed.

## Run

```bash
open index.html      # macOS
# or just double-click the file
```

> Note: marker/personnel data is simulated for the mockup.
