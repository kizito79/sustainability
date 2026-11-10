# CITIBIM Sustainability Dashboard

Interactive map of Nigeria's electricity infrastructure, resources, amenities and real time weather.
Static site (single `index.html`), built with Leaflet, Chart.js and OpenWeather.

## Deploy to Vercel

1. Import this repository in Vercel (New Project).
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy. `index.html` is served at `/`; the old `/sustainability.html` URL redirects to `/`.

Or from the CLI: `npx vercel --prod`.

## Run locally

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Data

Layer data is loaded on demand from `kizito79/REA_Dashbord` via `raw.githubusercontent.com`
(no CORS proxy needed). Layers whose files are missing (`mines.geojson`, `solar_radiance.geojson`)
or have no dataset yet show as greyed out in the sidebar.

OpenStreetMap is the default basemap; CARTO Light and Dark are available in the Weather tab.
