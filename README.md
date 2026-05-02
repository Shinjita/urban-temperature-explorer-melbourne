# 🌡️ Melbourne Urban Heat Island Explorer
### An Open-Source GIS Application

> An interactive, browser-based web map exploring the spatial relationship between Land Surface Temperature, building typology, and tree canopy coverage across Melbourne, Australia.

**Live map:** [https://YOUR_USERNAME.github.io/melbourne-heat-explorer](https://YOUR_USERNAME.github.io/melbourne-heat-explorer)

## 🗺️ What the Map Shows

| Layer | Description |
|---|---|
| 🌡️ **LST Zones** | Five-class land surface temperature choropleth derived from Landsat 8/9 Band 10. Classified using Natural Breaks (Jenks). |
| 🏢 **Building Footprints** | Melbourne City building polygons attributed by roof type (flat, hip, gable, pyramid) and average height. |
| 🌳 **Tree Canopy** | 1000+ trees fetched live from the City of Melbourne Urban Forest API, coloured by age class. |

## ✨ Features

- **LST Temperature Filter** — drag a slider to isolate temperature zones above a chosen threshold
- **Temperature Distribution Histogram** — bar chart showing SA2 area count per temperature class, matching the map's Spectral colour ramp
- **Live Tree API** — tree canopy data fetched at runtime from the Victorian Government CKAN DataStore API; not a static file
- **Tree Age Colouring** — young, mature, and over-mature trees rendered in distinct colours
- **Collapsible About Panel** — study purpose, aim, and dataset sources
- **Address Search** — Nominatim OpenStreetMap geocoder for locating suburbs and streets
- **GPS Locator** — centres the map on the user's current position
- **Dynamic Scale Bar** — updates automatically with zoom level
- **Attribution** — full data source credits at bottom centre

## 🎓 Academic Context

This map was produced as part of **GEOM2138/2151 — Cloud-Based Open-Source GIS** at **RMIT University**, 2026.

The practical exercise demonstrates a complete local-to-cloud GIS pipeline:

| Stage | Architecture label |
|---|---|
| Part 1 — PostGIS | Data Tier |
| Part 2 — QGIS + QGIS2Web | Processing Layer → Static Export |
| Part 3 — VS Code | Presentation Tier → Interactive Application |
| Part 4 — GitHub Pages | Local Application → Cloud Deployment |

---

## 👤 Author

**Shinjita Das**
RMIT University | GEOM2138/2151 | 2026

---

## 📄 Licence

Data licences:

- Landsat imagery: public domain (USGS/NASA)
- City of Melbourne Open Data: [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/)
- CartoDB basemap tiles: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — Data © OpenStreetMap contributors

Code in this repository is released under the [MIT Licence](https://opensource.org/licenses/MIT).
