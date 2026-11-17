# Run Tracker demo map

Map data for the web demo of [Run Tracker](https://github.com/Marc-Elz/run-tracker) at
https://marc-elz.github.io/run-tracker/. GitHub Pages serves these files at https://marc-elz.github.io/run-tracker-demo-map/, and the
demo loads `style.json` from there. It needs no API key.

Only two small areas are included, the places the demo shows: Utrecht (its sample runs) and a
spot in Amsterdam (its simulated GPS), at zoom levels 9 to 14, plus the region
around both at zoom 9 to 10 for the zoomed-out overview.

**Generated, not edited by hand.** Made with `scripts/make-demo-map.mjs` in the Run Tracker repo:

    node scripts/make-demo-map.mjs <clone of this repo> 20261117

from Protomaps planet build `20261117.pmtiles` (basemap 4.15.2) and
`@protomaps/basemaps` 5.7.2. Regenerating replaces everything here.

## Licences

The files here are not under the Run Tracker's MIT licence:

- `tiles/`: © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, available
  under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/), in the
  [Protomaps basemap](https://github.com/protomaps/basemaps) schema.
- `fonts/`: Noto Sans, under the SIL Open Font License, see `fonts/OFL.txt`.
- `sprites/`: from [protomaps/basemaps-assets](https://github.com/protomaps/basemaps-assets),
  derived from the MIT-licensed [tangrams/icons](https://github.com/tangrams/icons).
- `style.json`: generated with [@protomaps/basemaps](https://github.com/protomaps/basemaps)
  (BSD-3-Clause).
