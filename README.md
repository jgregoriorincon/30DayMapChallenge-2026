# #30DayMapChallenge 2026 with RustGIS

**English** · [Español](README.es.md) · [Gallery](https://jgregoriorincon.github.io/30DayMapChallenge-2026/)

The November 2026 maps, made end to end in [RustGIS](https://github.com/opengeos/RustGIS) in
the browser ([web.rustgis.app](https://web.rustgis.app)), with data on Bogotá, Barranquilla and
Colombia read straight from public web services.

Each day has:

- **The image** that was posted (`diaNN.webp`).
- **The project** (`diaNN.rgis`). Its link opens it in web.rustgis.app with the same layers,
  styles and layout as the image. Everyone opens their own copy.
- **The scripts** (`scripts/diaNN-a.txt` and `scripts/diaNN-b.txt`) that build the map from
  scratch in RustGIS's Script pane: part A requests the data from the services; once the layers
  arrive, part B processes them, styles them and builds the layout.

## Maps

| Day | Theme | Map | Open | Scripts | Data |
|---|---|---|---|---|---|
| 1 | Points | Bogotá's giants (Los gigantes de Bogotá) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia01.rgis) | [A](scripts/dia01-a.txt) · [B](scripts/dia01-b.txt) | Urban tree census, JBB / IDECA (CC BY 4.0); localities, Catastro Bogotá |
| 2 | Lines | Bogotá by bike (Bogotá en bicicleta) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia02.rgis) | [A](scripts/dia02-a.txt) · [B](scripts/dia02-b.txt) | Bike lane network (Red Biciusuarios), IDU / IDECA (CC BY 4.0) |
| 3 | Polygons | Barranquilla, block by block (Barranquilla, manzana por manzana) | [project](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia03.rgis) | [A](scripts/dia03-a.txt) · [B](scripts/dia03-b.txt) | Predominant socioeconomic stratum per block 2018, Esri Colombia from DANE data; municipal boundary, IGAC |

The maps themselves (titles, legends, sources) are in Spanish.

## Reproduce a day

1. Open [web.rustgis.app](https://web.rustgis.app) and the **Script** pane
   (Analyze › Geoprocessing).
2. Paste `scripts/diaNN-a.txt` and run it (Ctrl/⌘+Enter).
3. Wait until every layer shows up in the layers pane.
4. Paste `scripts/diaNN-b.txt` and run it.

The scripts request the data live, so the result may differ if a source changes. The `.rgis`
keeps the data as it was on the day of the map.

## Licences

- Scripts (`scripts/`) and the gallery (`index.html`): [MIT](LICENSE).
- Images (`diaNN.webp`) and projects (`diaNN.rgis`):
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), credited as
  "@jgregoriorincon, #30DayMapChallenge 2026, made with RustGIS".
- The data inside each `.rgis` keeps its source's licence (table above). Days with
  OpenStreetMap data: © OpenStreetMap contributors,
  [ODbL](https://opendatacommons.org/licenses/odbl/).
