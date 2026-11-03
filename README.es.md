# #30DayMapChallenge 2026 con RustGIS

[English](README.md) · **Español** · [Galería](https://jgregoriorincon.github.io/30DayMapChallenge-2026/)

Los mapas de noviembre de 2026, hechos de principio a fin en
[RustGIS](https://github.com/opengeos/RustGIS) desde el navegador
([web.rustgis.app](https://web.rustgis.app)), con datos de Bogotá, Barranquilla y Colombia
que se leen directamente de servicios públicos.

Cada día tiene:

- **La imagen** que se publicó (`diaNN.webp`).
- **El proyecto** (`diaNN.rgis`). El enlace lo abre en web.rustgis.app con las mismas capas,
  estilos y layout de la imagen. Cada persona abre su propia copia.
- **Los scripts** (`scripts/diaNN-a.txt` y `scripts/diaNN-b.txt`) que construyen el mapa desde
  cero en el panel Script de RustGIS: la parte A pide los datos a los servicios; cuando las
  capas llegan, la parte B procesa, da estilo y arma el layout.

## Mapas

| Día | Tema | Mapa | Abrir | Scripts | Datos |
|---|---|---|---|---|---|
| 1 | Points | Los gigantes de Bogotá | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia01.rgis) | [A](scripts/dia01-a.txt) · [B](scripts/dia01-b.txt) | Censo del arbolado urbano, JBB / IDECA (CC BY 4.0); localidades, Catastro Bogotá |
| 2 | Lines | Bogotá en bicicleta | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia02.rgis) | [A](scripts/dia02-a.txt) · [B](scripts/dia02-b.txt) | Red Biciusuarios, IDU / IDECA (CC BY 4.0) |
| 3 | Polygons | Barranquilla, manzana por manzana | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/dia03.rgis) | [A](scripts/dia03-a.txt) · [B](scripts/dia03-b.txt) | Estrato predominante por manzana 2018, Esri Colombia con datos del DANE; límite municipal, IGAC |

## Cómo reproducir un día

1. Abrir [web.rustgis.app](https://web.rustgis.app) y el panel **Script**
   (Analyze › Geoprocessing).
2. Pegar `scripts/diaNN-a.txt` y correrlo (Ctrl/⌘+Enter).
3. Esperar a que todas las capas aparezcan en el panel de capas.
4. Pegar `scripts/diaNN-b.txt` y correrlo.

Los datos se piden en vivo a los servicios, así que el resultado puede variar si la fuente
cambia. El `.rgis` guarda los datos tal como estaban el día del mapa.

## Licencias

- Scripts (`scripts/`) y la galería (`index.html`): [MIT](LICENSE).
- Imágenes (`diaNN.webp`) y proyectos (`diaNN.rgis`):
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), citando
  "@jgregoriorincon, #30DayMapChallenge 2026, hecho con RustGIS".
- Los datos dentro de cada `.rgis` conservan la licencia de su fuente (tabla de arriba).
  Los días con datos de OpenStreetMap: © colaboradores de OpenStreetMap,
  [ODbL](https://opendatacommons.org/licenses/odbl/).
