# #30DayMapChallenge 2026 with RustGIS

**English** · [Español](README.es.md) · [Gallery](https://jgregoriorincon.github.io/30DayMapChallenge-2026/)

The November 2026 maps, made end to end in [RustGIS](https://github.com/opengeos/RustGIS) in
the browser ([web.rustgis.app](https://web.rustgis.app)), with data on Bogotá, Barranquilla and
Colombia read straight from public web services.

Each day has:

- **The image** that was posted and the PDF RustGIS exported, in Spanish and English
  (`results/day-NN/day-NN-es.webp`, `day-NN-en.webp`, `day-NN-es.pdf`, `day-NN-en.pdf`).
- **The project** (`results/day-NN/day-NN.rgis`). Its link opens it in web.rustgis.app with the same layers
  and styles as the image, and both layouts: "Dia NN" (Spanish) and "Day NN" (English). Everyone opens their own copy.
- **The scripts** that build it from scratch in RustGIS's Script pane:
  1. `scripts/day-NN/01-data.txt` (data): basemap, map extent and the requests to the services.
  2. `scripts/day-NN/02-view.txt` (view): processing and styling; the map is finished here.
  3. `scripts/day-NN/03-layout.txt` (layout): title, legend, scale, sources.
  4. `scripts/day-NN/04-english.txt` (English layout): the same layout with its texts in English, on the
     same map. Layer names and legend classes keep the data's Spanish names.

## Maps

| Day | Theme | Map | Open | Scripts | Data |
|---|---|---|---|---|---|
| 1 | Points | Bogotá's giants: its tallest trees (Los gigantes de Bogotá) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-01/day-01.rgis) | [1](scripts/day-01/01-data.txt) · [2](scripts/day-01/02-view.txt) · [3](scripts/day-01/03-layout.txt) · [4](scripts/day-01/04-english.txt) | Urban tree census, JBB / IDECA (CC BY 4.0); basemap: Mapa Base Bogotá, IDECA |
| 2 | Lines | Bogotá by bike (Bogotá en bicicleta) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-02/day-02.rgis) | [1](scripts/day-02/01-data.txt) · [2](scripts/day-02/02-view.txt) · [3](scripts/day-02/03-layout.txt) · [4](scripts/day-02/04-english.txt) | Bike lane network (Red Biciusuarios), IDU / IDECA (CC BY 4.0); basemap: Mapa base azul, IDECA |
| 3 | Polygons | Barranquilla, block by block (Barranquilla, manzana por manzana) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-03/day-03.rgis) | [1](scripts/day-03/01-data.txt) · [2](scripts/day-03/02-view.txt) · [3](scripts/day-03/03-layout.txt) · [4](scripts/day-03/04-english.txt) | Predominant socioeconomic stratum per block 2018, DANE / Esri Colombia; municipal boundary, IGAC; basemap: Mi Ciudad, Alcaldía de Barranquilla |
| 4 | Clusters | Bogotá's black spots: fatal road crash hotspots (Los puntos negros de Bogotá) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-04/day-04.rgis) | [1](scripts/day-04/01-data.txt) · [2](scripts/day-04/02-view.txt) · [3](scripts/day-04/03-layout.txt) · [4](scripts/day-04/04-english.txt) | Fatal road crashes 2016–2025, Secretaría Distrital de Movilidad (SIMUR; no licence declared); basemap: Mapa base azul, IDECA |
| 5 | Senses: Sight | What can you see from Monserrate? (¿Qué se ve desde Monserrate?) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-05/day-05.rgis) | [1](scripts/day-05/01-data.txt) · [2](scripts/day-05/02-view.txt) · [3](scripts/day-05/03-layout.txt) · [4](scripts/day-05/04-english.txt) | Digital Terrain Model of Bogotá D.C. 2025, IDECA (CC BY 4.0); basemap: Mapa base azul, IDECA |
| 6 | Vintage | Cartagena de Indias, as Herrera drew it (Cartagena de Indias, según Herrera) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-06/day-06.rgis) | [1](scripts/day-06/01-data.txt) · [2](scripts/day-06/02-view.txt) · [3](scripts/day-06/03-layout.txt) · [4](scripts/day-06/04-english.txt) | Plan of Cartagena by Juan de Herrera y Sotomayor (18th c.), Bibliothèque nationale de France / Gallica (public domain), via Wikimedia Commons; today's bastions and basemap: © OpenStreetMap contributors (ODbL) |
| 7 | 10 minute map | An afternoon of clouds over Colombia (Una tarde de nubes sobre Colombia) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-07/day-07.rgis) | [1](scripts/day-07/01-data.txt) · [2](scripts/day-07/02-view.txt) · [3](scripts/day-07/03-layout.txt) · [4](scripts/day-07/04-english.txt) | NOAA GOES-East ABI, GeoColor product (CIRA/NOAA), served by NASA GIBS (accessed 2026-11-06; GIBS keeps these images for about 3 months, so the project may later open without them); boundary: geoBoundaries (CC0) |

Each map comes in Spanish and in English; the legend classes keep the data's Spanish names.

## Reproduce a day

1. Open [web.rustgis.app](https://web.rustgis.app) and the **Script** pane
   (Analyze › Geoprocessing).
2. Paste `scripts/day-NN/01-data.txt` and run it (Ctrl/⌘+Enter).
3. Wait until every layer shows up in the layers pane: in the browser the downloads run in the
   background, and script 2 needs them.
4. Paste and run `scripts/day-NN/02-view.txt`, then `scripts/day-NN/03-layout.txt` and
   `scripts/day-NN/04-english.txt`.

The scripts request the data live, so the result may differ if a source changes. The `.rgis`
keeps the data as it was on the day of the map.

## Licences

- Scripts (`scripts/`) and the gallery (`index.html`): [MIT](LICENSE).
- Images (`results/day-NN/day-NN-{es,en}.webp`, `results/day-NN/day-NN-{es,en}.pdf`) and projects (`results/day-NN/day-NN.rgis`):
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), credited as
  "@jgregoriorincon, #30DayMapChallenge 2026, made with RustGIS".
- The data inside each `.rgis` keeps its source's licence (table above). Days with
  OpenStreetMap data: © OpenStreetMap contributors,
  [ODbL](https://opendatacommons.org/licenses/odbl/).
