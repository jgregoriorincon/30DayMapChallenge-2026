# Day 21 data: Providencia after Hurricane Iota

Copies served from GitHub Pages because their original servers don't send CORS headers or can't
be queried by date from RustGIS web. Each file keeps its source licence.

| File | What | Source | Licence |
|---|---|---|---|
| `osm-edificios-2020-11-15.geojson` | 1,988 building footprints in Providencia and Santa Catalina as OpenStreetMap had them on 15 November 2020, the day before Iota (fields `osm_id`, `building`) | OpenStreetMap, Overpass API with `[date:"2020-11-15T00:00:00Z"]`, bbox 13.30, -81.42, 13.42, -81.33 | © OpenStreetMap contributors, [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/) |
| `unosat-danos-2020-11-21.geojson` | 1,110 damaged structures detected on a WorldView-2 image of 21 November 2020: 1,100 `Destroyed` and 10 `Possible Damage` (fields `dano`, `fecha`) | UNITAR-UNOSAT, TC20201123COL, "Damage Assessment in Providencia Island, Providencia and Santa Catalina Department, Colombia as of 21 November 2020" ([HDX](https://data.humdata.org/dataset/damage-assessment-in-providencia-island-providencia-and-santa-catalina-department-colombia)) | CC BY-SA |
| `unosat-nubes-2020-11-21.geojson` | The cloud mask of the same image: areas UNOSAT could not analyse | Same | CC BY-SA |

UNOSAT's own description: "Within the Island boundary, UNITAR-UNOSAT identified in the cloud-free
zones 1,110 damaged structures. Taking into account the pre-building footprints provided by
Humanitarian OpenStreetMap, this represents about 90% of the total number of structures within the
analyzed cloud-free areas."
