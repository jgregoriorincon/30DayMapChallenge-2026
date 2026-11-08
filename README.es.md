# #30DayMapChallenge 2026 con RustGIS

[English](README.md) · **Español** · [Galería](https://jgregoriorincon.github.io/30DayMapChallenge-2026/)

Los mapas de noviembre de 2026, hechos de principio a fin en
[RustGIS](https://github.com/opengeos/RustGIS) desde el navegador
([web.rustgis.app](https://web.rustgis.app)), con datos de Colombia y de sus ciudades
(Bogotá, Barranquilla, Cartagena, Medellín, Bucaramanga, Cali y Cúcuta) que se leen directamente de servicios públicos.

Por [Jose Gregorio Rincon Albarracin](https://github.com/jgregoriorincon), ingeniero catastral y geodesta, contribuidor de RustGIS · [LinkedIn](https://www.linkedin.com/in/jgregoriorincon/)

Cada día tiene:

- **La imagen** que se publicó y el PDF que exportó RustGIS, en español y en inglés
  (`results/day-NN/day-NN-es.webp`, `day-NN-en.webp`, `day-NN-es.pdf`, `day-NN-en.pdf`).
- **El proyecto** (`results/day-NN/day-NN.rgis`). El enlace lo abre en web.rustgis.app con las mismas capas
  y estilos de la imagen, y los dos layouts: "Dia NN" (español) y "Day NN" (inglés). Cada persona abre su propia copia.
- **Los scripts** que lo construyen desde cero en el panel Script de RustGIS:
  1. `scripts/day-NN/01-data.txt`: mapa base, encuadre y consultas a los servicios.
  2. `scripts/day-NN/02-view.txt`: proceso y estilo; aquí el mapa queda terminado.
  3. `scripts/day-NN/03-layout.txt`: título, leyenda, escala y fuentes.
  4. `scripts/day-NN/04-english.txt`: el mismo layout con sus textos en inglés, sobre el mismo mapa.
     Las capas y las clases de la leyenda conservan los nombres de los datos, en español.

## Mapas

| Día | Tema | Mapa | Abrir | Scripts | Datos |
|---|---|---|---|---|---|
| 1 | Points | Los gigantes de Bogotá | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-01/day-01.rgis) | [1](scripts/day-01/01-data.txt) · [2](scripts/day-01/02-view.txt) · [3](scripts/day-01/03-layout.txt) · [4](scripts/day-01/04-english.txt) | Censo del arbolado urbano, JBB / IDECA (CC BY 4.0); mapa base: Mapa Base Bogotá, IDECA |
| 2 | Lines | Bogotá en bicicleta | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-02/day-02.rgis) | [1](scripts/day-02/01-data.txt) · [2](scripts/day-02/02-view.txt) · [3](scripts/day-02/03-layout.txt) · [4](scripts/day-02/04-english.txt) | Red Biciusuarios, IDU / IDECA (CC BY 4.0); mapa base: Mapa base azul, IDECA |
| 3 | Polygons | Barranquilla, manzana por manzana | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-03/day-03.rgis) | [1](scripts/day-03/01-data.txt) · [2](scripts/day-03/02-view.txt) · [3](scripts/day-03/03-layout.txt) · [4](scripts/day-03/04-english.txt) | Estrato predominante por manzana 2018, DANE / Esri Colombia; límite municipal, IGAC; mapa base: Mi Ciudad, Alcaldía de Barranquilla |
| 4 | Clusters | Los puntos negros de Bogotá | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-04/day-04.rgis) | [1](scripts/day-04/01-data.txt) · [2](scripts/day-04/02-view.txt) · [3](scripts/day-04/03-layout.txt) · [4](scripts/day-04/04-english.txt) | Siniestros viales con muertos 2016–2025, Secretaría Distrital de Movilidad (SIMUR; sin licencia declarada); mapa base: Mapa base azul, IDECA |
| 5 | Senses: Sight | ¿Qué se ve desde Monserrate? | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-05/day-05.rgis) | [1](scripts/day-05/01-data.txt) · [2](scripts/day-05/02-view.txt) · [3](scripts/day-05/03-layout.txt) · [4](scripts/day-05/04-english.txt) | Modelo Digital de Terreno de Bogotá D.C. 2025, IDECA (CC BY 4.0); mapa base: Mapa base azul, IDECA |
| 6 | Vintage | Cartagena de Indias, según Herrera | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-06/day-06.rgis) | [1](scripts/day-06/01-data.txt) · [2](scripts/day-06/02-view.txt) · [3](scripts/day-06/03-layout.txt) · [4](scripts/day-06/04-english.txt) | Plano de Cartagena de Juan de Herrera y Sotomayor (siglo XVIII), Bibliothèque nationale de France / Gallica (dominio público), vía Wikimedia Commons; baluartes de hoy y mapa base: © colaboradores de OpenStreetMap (ODbL) |
| 7 | 10 minute map | Una tarde de nubes sobre Colombia | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-07/day-07.rgis) | [1](scripts/day-07/01-data.txt) · [2](scripts/day-07/02-view.txt) · [3](scripts/day-07/03-layout.txt) · [4](scripts/day-07/04-english.txt) | NOAA GOES-East ABI, producto GeoColor (CIRA/NOAA), servido por NASA GIBS (consultado el 2026-11-06; GIBS guarda estas imágenes unos 3 meses, así que más adelante el proyecto puede abrir sin ellas); límite: geoBoundaries (CC0) |
| 8 | Utopia | La utopía del 3-30-300 en Medellín | [proyecto](https://web.rustgis.app/?project=https://jgregoriorincon.github.io/30DayMapChallenge-2026/results/day-08/day-08.rgis) | [1](scripts/day-08/01-data.txt) · [2](scripts/day-08/02-view.txt) · [3](scripts/day-08/03-layout.txt) · [4](scripts/day-08/04-english.txt) | Alcaldía de Medellín, Departamento Administrativo de Planeación (GeoMedellín), CC BY-SA 4.0: ortofoto de noviembre de 2024, manzanas, espacio público existente y comunas; mapa base: Alcaldía de Medellín. **Este mapa y su proyecto: CC BY-SA 4.0** |

## Cómo reproducir un día

1. Abrir [web.rustgis.app](https://web.rustgis.app) y el panel **Script**
   (Analyze › Geoprocessing).
2. Pegar `scripts/day-NN/01-data.txt` y correrlo (Ctrl/⌘+Enter).
3. Esperar a que todas las capas aparezcan en el panel de capas: en el navegador las descargas
   siguen en segundo plano, y el script 2 las necesita.
4. Pegar y correr `scripts/day-NN/02-view.txt`, y luego `scripts/day-NN/03-layout.txt` y
   `scripts/day-NN/04-english.txt`.

Los datos se piden en vivo a los servicios, así que el resultado puede variar si la fuente
cambia. El `.rgis` guarda los datos tal como estaban el día del mapa.

## Licencias

- Scripts (`scripts/`) y la galería (`index.html`): [MIT](LICENSE).
- Imágenes (`results/day-NN/day-NN-{es,en}.webp`, `results/day-NN/day-NN-{es,en}.pdf`) y proyectos (`results/day-NN/day-NN.rgis`):
  [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), citando
  "@jgregoriorincon, #30DayMapChallenge 2026, hecho con RustGIS". Excepción: el día 8 va con
  [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), porque así vienen sus datos.
- Los datos dentro de cada `.rgis` conservan la licencia de su fuente (tabla de arriba).
  Los días con datos de OpenStreetMap: © colaboradores de OpenStreetMap,
  [ODbL](https://opendatacommons.org/licenses/odbl/).
