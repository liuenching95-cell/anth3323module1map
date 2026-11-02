# ANTH3323 Module1 — B11 Photo Map

Interactive web map of 22 ethnographic photographs from Shek Mun Kap (石門甲) and Fong Yuen Village (芳園村), Lantau Island, Hong Kong. Photographs taken in January 1992 by 顏孔昭, 張振江, and 黎振翔.

## Live site

After enabling GitHub Pages (see below), the site will be available at:

```
https://<your-username>.github.io/<repo-name>/index_custom_v1.html
```

## Pages

| File | Description |
|---|---|
| `index_custom_v1.html` | **Custom interactive map** — three-pane layout with filters, Leaflet map, and photo detail panel |
| `index.html` | Original qgis2web export (standard popup-based interface) |

## Features (index_custom_v1.html)

- **Left panel**: Dynamic filters by Place Name, Photo Subject, and Location Precision with Select All / Clear buttons and live record count
- **Center**: Leaflet map with aerial raster overlay, marker clustering, and highlighted selection
- **Right panel**: Click any marker to view the photograph and metadata (file name, place, date, subject, direction, location precision/source, notes)
- **Responsive**: Works on desktop, tablet, and mobile
- **Lightbox**: Click any photo in the detail panel to view it full-resolution

## Data

- **22 photo points** from `data/Module1DotsB11_1.js` (GeoJSON, WGS84)
- **Aerial imagery** from `data/omp100_2025_clipped_0.png`
- **Photographs** in `images/` (22 JPG files)

## How to publish on GitHub Pages

1. Create a new repository on [github.com](https://github.com/new)
2. Upload all files from this folder (drag-and-drop or `git push`)
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` (or `master`) branch, folder `/ (root)`
6. Click **Save**
7. Wait 1–2 minutes, then visit the URL shown at the top of the Pages settings

## Tech

- [Leaflet](https://leafletjs.com/) — mapping library
- [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster) — marker clustering
- [qgis2web](https://github.com/qgis2web/qgis2web) — original export from QGIS
