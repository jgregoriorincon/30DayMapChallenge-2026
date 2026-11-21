# Day 21 data: Pereira after the 10 August 2026 earthquake

A copy served from GitHub Pages because RustGIS web downloads from OpenStreetMap only the features
that carry `building=*`, and the buildings the earthquake took no longer do.

| File | What | Source | Licence |
|---|---|---|---|
| `osm-edificios-pereira-2026-11-20.geojson` | 112,329 building footprints in Pereira and Dosquebradas (bbox 4.70, -75.85, 4.95, -75.55) with their state tags: `building`, `destruida` (`destroyed:building`), `demolida` (`demolished:building`) and `sismo` (`damage:event`) | OpenStreetMap, Overpass API, 20 November 2026: ways with `building`, `destroyed:building` or `demolished:building` | © OpenStreetMap contributors, [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/) |

The state tags come from the OSM Colombia / AC3 response
([HOT Tasking Manager project 67260](https://tasks.hotosm.org/projects/67260)), which reviewed Pereira
on a post-earthquake FlyNorth drone orthophoto and on ground reports sent through ChatMap. A building
that collapsed becomes `destroyed:building=*`, and one demolished later becomes
`demolished:building=*`, both with `damage:event=2026ColombiaEarthquake-Palmar`. The data changes
daily while the project is open: this copy is the state on 20 November 2026.
