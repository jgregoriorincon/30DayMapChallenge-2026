# Day 21 data: Pereira after the 10 August 2026 earthquake

A copy served from GitHub Pages because RustGIS web downloads from OpenStreetMap only the features
that carry `building=*`, and the buildings the earthquake took no longer do.

| File | What | Source | Licence |
|---|---|---|---|
| `osm-edificios-pereira-2026-11-20.geojson` | 112,329 building footprints in Pereira and Dosquebradas (bbox 4.70, -75.85, 4.95, -75.55) with their state tags: `building`, `destruida` (`destroyed:building`), `demolida` (`demolished:building`) and `sismo` (`damage:event`) | OpenStreetMap, Overpass API, 20 November 2026: ways with `building`, `destroyed:building` or `demolished:building` | © OpenStreetMap contributors, [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/) |
| `hot-67260-area.geojson` | The area of interest of HOT Tasking Manager project 67260, the part of central Pereira reviewed on the drone orthophoto. 451 of the 455 lost buildings and 33,678 of the 41,999 buildings OSM has in the municipality fall inside it | [HOT Tasking Manager API](https://tasking-manager-production-api.hotosm.org/api/v2/projects/67260/queries/aoi/), 21 November 2026 | HOT Tasking Manager project data |

The state tags come from the OSM Colombia / AC3 response
([HOT Tasking Manager project 67260](https://tasks.hotosm.org/projects/67260)), which reviewed Pereira
on a post-earthquake FlyNorth drone orthophoto and on ground reports sent through ChatMap. A building
that collapsed becomes `destroyed:building=*`, and one demolished later becomes
`demolished:building=*`, both with `damage:event=2026ColombiaEarthquake-Palmar`. The data changes
daily while the project is open: this copy is the state on 20 November 2026.
