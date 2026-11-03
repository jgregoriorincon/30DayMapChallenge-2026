# #30DayMapChallenge 2026 con RustGIS

[English](README.md) · **Español** · [Galería](https://jgregoriorincon.github.io/30DayMapChallenge-2026/)

Los mapas de noviembre de 2026, hechos de principio a fin en
[RustGIS](https://github.com/opengeos/RustGIS) desde el navegador
([web.rustgis.app](https://web.rustgis.app)), con datos de Bogotá, Barranquilla y Colombia
que se leen directamente de servicios públicos.

Cada día tiene:

- **La imagen** que se publicó (`results/day-NN/day-NN.webp`) y el PDF que exportó RustGIS (`results/day-NN/day-NN.pdf`).
- **El proyecto** (`results/day-NN/day-NN.rgis`). El enlace lo abre en web.rustgis.app con las mismas capas,
  estilos y layout de la imagen. Cada persona abre su propia copia.
- **Los scripts** que lo construyen desde cero en el panel Script de RustGIS:
  1. `scripts/day-NN/01-data.txt`: mapa base, encuadre y consultas a los servicios.
  2. `scripts/day-NN/02-view.txt`: proceso y estilo; aquí el mapa queda terminado.
  3. `scripts/day-NN/03-layout.txt`: título, leyenda, escala y fuentes.

## Mapas

| Día | Tema | Mapa | Abrir | Scripts | Datos |
|---|---|---|---|---|---|
| 1 | Points | Los gigantes de Bogotá | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-01/day-01.rgis) | [1](scripts/day-01/01-data.txt) · [2](scripts/day-01/02-view.txt) · [3](scripts/day-01/03-layout.txt) | Censo del arbolado urbano, JBB / IDECA (CC BY 4.0); mapa base: Mapa Base Bogotá, IDECA |
| 2 | Lines | Bogotá en bicicleta | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-02/day-02.rgis) | [1](scripts/day-02/01-data.txt) · [2](scripts/day-02/02-view.txt) · [3](scripts/day-02/03-layout.txt) | Red Biciusuarios, IDU / IDECA (CC BY 4.0) |
| 3 | Polygons | Barranquilla, manzana por manzana | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-03/day-03.rgis) | [1](scripts/day-03/01-data.txt) · [2](scripts/day-03/02-view.txt) · [3](scripts/day-03/03-layout.txt) | Estrato predominante por manzana 2018, Esri Colombia con datos del DANE; límite municipal, IGAC |

## Cómo reproducir un día

1. Abrir [web.rustgis.app](https://web.rustgis.app) y el panel **Script**
   (Analyze › Geoprocessing).
2. Pegar `scripts/day-NN/01-data.txt` y correrlo (Ctrl/⌘+Enter).
3. Esperar a que todas las capas aparezcan en el panel de capas: en el navegador las descargas
   siguen en segundo plano, y el script 2 las necesita.
4. Pegar y correr `scripts/day-NN/02-view.txt`, y luego `scripts/day-NN/03-layout.txt`.

Los datos se piden en vivo a los servicios, así que el resultado puede variar si la fuente
cambia. El `.rgis` guarda los datos tal como estaban el día del mapa.

## Licencias

- Scripts (`scripts/`) y la galería (`index.html`): [MIT](LICENSE).
- Imágenes (`results/day-NN/day-NN.webp`, `results/day-NN/day-NN.pdf`) y proyectos (`results/day-NN/day-NN.rgis`):
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), citando
  "@jgregoriorincon, #30DayMapChallenge 2026, hecho con RustGIS".
- Los datos dentro de cada `.rgis` conservan la licencia de su fuente (tabla de arriba).
  Los días con datos de OpenStreetMap: © colaboradores de OpenStreetMap,
  [ODbL](https://opendatacommons.org/licenses/odbl/).
