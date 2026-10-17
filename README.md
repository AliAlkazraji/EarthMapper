
# EarthMapper

**EarthMapper** is a free, non-commercial Windows desktop mapping application for viewing, creating, editing, analyzing, and exporting geospatial data in a simple, practical environment.

It is designed for users who need accessible GIS, surveying, remote sensing, and terrain tools without requiring a full GIS package for every task.
<img width="1919" height="1034" alt="image" src="https://github.com/user-attachments/assets/8f8ce18b-c442-4b02-8b22-f9aeebba5a03" />


## Key Features

- **2D and 3D mapping** with online and offline workflows, including 3D globe and terrain visualization.
- Import and work with **KML/KMZ, Shapefile (SHP), DXF, CSV, GeoTIFF**, and other common geospatial formats.
- Export vector data to **KML/KMZ, SHP, DXF, CSV**, and other supported formats.
- Export maps as **PNG, JPEG, TIFF, and GeoTIFF**.
- Draw and edit **points, lines, polygons, rectangles, squares, circles, and ellipses**.
- Precise drawing using **Distance, Direction/Azimuth, Distance + Direction, Angle, and ΔX/ΔY** constraints.
- **Identify, Select, Move, Split, Buffer, Measure, Snap, Undo**, and other geometry-editing tools.
- **Line Division** by equal parts or specified segment length, with optional division points.
- **Area Division** for fixed-size parcels, equal-area parcels, and equal-width divisions.
- Coordinate support for **WGS 84 Geographic, UTM, and MGRS**.
- Custom **Geographic, UTM, and MGRS grids**, including manual spacing and advanced grid-point labeling.

### Terrain and Elevation

- **Elevation profiles, point elevations, DEM generation, contours, and 3D terrain** using multiple elevation sources.
- Create elevation profiles from **lines or point layers**, using distance, stationing, or point-number X-axis modes.
- Compare up to **three elevation sources** in one profile with source-difference statistics.
- Generate **DEMs and contour lines** from Mapterhorn elevation data or user point layers using **IDW or Kriging**.
- **FABDEM Explorer** for finding, selecting, downloading, and importing approximately 30 m bare-earth DEM tiles using interactive map footprints.

### Satellite Imagery and Remote Sensing

- **Sentinel-2 Explorer** for searching satellite scenes by area, acquisition date, and cloud cover.
- Display Sentinel-2 scene footprints and temporary previews on the map.
- Visualize **10 m true-color Sentinel-2 RGB imagery online**.
- Download selected Sentinel-2 spectral bands individually or as a **multiband GeoTIFF**.
- Generate and download scientific products, including **NDVI, NDWI, RGB composites, and scene-classification outputs**.
- Choose output resolution and resampling methods when exporting multiband GeoTIFFs.
- **Esri Wayback historical imagery** with location-specific acquisition dates where available.
- **EOxCloudless Sentinel-2 annual mosaics** integrated into historical imagery and basemap selection.
- **Overture Maps** download workflows for supported vector datasets.

### Raster Visualization

- **Single-band and multiband raster symbology**, including RGB channel assignment and color ramps.
- Multiple display stretch methods:
  - Minimum–Maximum
  - Standard Deviation (1σ, 1.5σ, 2σ, 2.5σ, 3σ)
  - Percent Clip
  - Custom Range
- **Native-resolution tiled GeoTIFF rendering** for detailed raster visualization.
- Automatic, on-demand **raster pyramid caching** to improve performance when navigating large imagery.
- Docked symbology editors with **Apply**, **OK**, and **Cancel** controls.
- Raster and vector symbology settings can be adjusted while keeping the map accessible.

### GeoAI and Spatial Analysis

- **GeoAI object detection** on imported GeoTIFF imagery using a built-in aerial oriented-bounding-box (OBB) model or a custom ONNX model.
- Native-resolution tiled GeoAI processing with class selection, overlap handling, progress display, and georeferenced detection output.
- Shapefile CRS detection and supported reprojection during import.
- Advanced vector styling, labeling, attribute editing, feature-level styling, and project saving.
- Multi-feature summaries with geometry statistics, extents, detailed reports, and HTML export.

## Free to Use

**EarthMapper is provided free of charge as a non-commercial application.**

The application itself is free. Third-party libraries, imagery, elevation datasets, map services, AI models, and other data sources retain their respective licenses, attribution requirements, usage limits, and terms of service.

Users are responsible for ensuring that their use of third-party resources complies with the applicable terms, particularly when using data for commercial projects or redistribution.

## Acknowledgements

EarthMapper makes use of technologies, datasets, and services developed by the wider open-source, geospatial, surveying, and Earth-observation communities.

Special thanks to the following projects, organizations, researchers, and contributors.

### Mapping Platforms and Basemaps

- [Leaflet](https://leafletjs.com/) — interactive 2D web mapping.
- [MapLibre GL JS](https://maplibre.org/) — interactive maps, 3D globe rendering, and terrain visualization.
- [Esri](https://www.esri.com/) — World Imagery, Topographic basemaps, and Wayback historical imagery services.
- [OpenStreetMap](https://www.openstreetmap.org/) contributors — collaborative geographic data and related basemaps.
- [Google Maps Platform](https://mapsplatform.google.com/) — optional Google mapping and imagery services, subject to Google's terms.

### Satellite Imagery and Imagery Catalogs

- [Copernicus Sentinel-2](https://dataspace.copernicus.eu/) — multispectral Earth-observation imagery made available through the European Union's Copernicus programme, with support from the European Space Agency (ESA). EarthMapper uses Sentinel-2 imagery for spectral-band viewing and products such as NDVI and NDWI.
- [Element 84 Earth Search](https://element84.com/earth-search/) — STAC-based search and discovery of Sentinel-2 and other openly available Earth-observation data.
- [Taylor Geospatial / Source Cooperative — Sentinel-2 STAC-GeoParquet](https://source.coop/tge-labs/s2-stac-geoparquet) — cloud-native Sentinel-2 scene indexing and metadata access. This catalog indexes imagery; the original satellite assets remain hosted separately.
- [AWS Registry of Open Data — Sentinel-2 COGs](https://registry.opendata.aws/sentinel-2-l2a-cogs/) — cloud-optimized Sentinel-2 imagery assets used by supported data-access workflows.
- [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/) — geospatial data catalog and services used for supported online imagery-access workflows.
- [Development Seed — TiTiler](https://github.com/developmentseed/titiler) — open-source dynamic raster tiling technology used by compatible online imagery services.
- [Radiant Earth](https://www.radiant.earth/) — geospatial open-data and raster-service initiatives relevant to online imagery access.
- [EOxCloudless by EOX IT Services GmbH](https://cloudless.eox.at/) — Sentinel-2 cloudless basemaps and annual historical mosaics. These mosaics contain modified Copernicus Sentinel data and have year-specific attribution requirements.

### Elevation and Geospatial Datasets

- [Mapterhorn](https://www.mapterhorn.com/) — online elevation and terrain data used for 3D terrain, profiles, and elevation sampling.
- [FABDEM v1.2 — University of Bristol](https://research-information.bris.ac.uk/en/datasets/fabdem-v1-2/) — approximately 30 m global elevation data with forest and building height effects removed from the Copernicus GLO-30 DEM. Credit to Laurence Hawker, Jeff Neal, their collaborators, and the institutions involved in developing and publishing FABDEM.
- [Overture Maps Foundation](https://overturemaps.org/) — openly available geospatial datasets, including buildings, transportation, places, and other supported themes. Some source data require additional attribution, including OpenStreetMap contributors.

### Software Frameworks and Data Processing

- [Microsoft .NET / WPF](https://dotnet.microsoft.com/) — EarthMapper's Windows desktop application framework.
- [Microsoft Edge WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) — embedding web-based mapping engines in the desktop application.
- [NetTopologySuite](https://github.com/NetTopologySuite/NetTopologySuite) — geometry processing and spatial operations.
- [netDxf](https://github.com/haplokuon/netDxf) — DXF reading and writing support.
- [BitMiracle LibTiff.NET](https://github.com/BitMiracle/libtiff.net) — TIFF/GeoTIFF reading and writing support.
- [DuckDB](https://duckdb.org/) — analytical queries and processing workflows for cloud-native geospatial and Parquet datasets.


### GeoAI and Aerial Object Detection

EarthMapper integrates AI-powered object detection and segmentation tools for aerial imagery, satellite imagery, and GeoTIFF raster analysis.

#### Frameworks, Datasets, and Models

- [Microsoft ONNX Runtime](https://onnxruntime.ai/) — Local neural-network inference.
- [Ultralytics](https://www.ultralytics.com/) — YOLO object-detection and segmentation framework.
- [DOTA Dataset](https://captain-whu.github.io/DOTA/) — Aerial imagery dataset used for training and evaluating oriented object-detection models.
- [YOLO26-DOTA-v2](https://github.com/JustinVladut/YOLO26-DOTA-v2) by JustinVladut — Source project for EarthMapper's built-in aerial-oriented object-detection model.
- [TreeSensing](https://github.com/flyingvaibhav/TreeSensing) by flyingvaibhav — YOLO-based tree detection and counting project, referenced for EarthMapper's tree detection functionality.
- [YOLOv8n Building Segmentation](https://huggingface.co/keremberke/yolov8n-building-segmentation) by keremberke — Building instance-segmentation model reference for identifying buildings in aerial imagery.
- [Segment Anything Model 2 (SAM 2)](https://github.com/facebookresearch/sam2) by Meta AI — Interactive image segmentation using positive and negative point prompts.
- [Segment Anything Model 3 (SAM 3)](https://github.com/facebookresearch/sam3) by Meta AI — Text-prompt-guided object detection and instance segmentation.

#### GeoAI Capabilities

- **Aerial Object Detection:** Oriented bounding-box detection for aircraft, ships, storage tanks, vehicles, bridges, harbors, airports, helipads, and other DOTA categories.
- **Tree Detection:** Automatic tree detection and localization in aerial and satellite imagery.
- **Building Segmentation:** Detection and segmentation of buildings from high-resolution imagery.
- **SAM 2 Segmentation:** Interactive object segmentation using positive and negative point selections.
- **SAM 3 Segmentation:** Optional text-guided object detection and instance segmentation.
- **GIS Integration:** Convert detection and segmentation results into GIS layers for mapping, symbology, attribute analysis, and spatial processing.

#### Licensing and Attribution

EarthMapper acknowledges the developers, researchers, and organizations behind these frameworks, datasets, and AI models.

All third-party components remain subject to their respective licenses and terms of use.

- **SAM 2:** Apache License 2.0.
- **SAM 3:** Meta SAM License.
- **YOLO26-DOTA-v2:** Refer to the upstream repository's license.
- **Ultralytics-based models:** Applicable model and framework licenses must be respected.

The provenance and redistribution rights of supplied model weights should be independently verified.

These acknowledgments do not imply endorsement of or affiliation with EarthMapper by the original developers.


## Third-Party Services and Licensing

EarthMapper provides access to third-party imagery, basemaps, terrain, elevation, vector datasets, and AI technologies. Their licenses apply independently of EarthMapper's free distribution.

- **Sentinel-2 / Copernicus:** Sentinel data and derived imagery must follow the applicable [Copernicus data-use terms](https://dataspace.copernicus.eu/). Appropriate source acknowledgment should be retained in imagery exports and publications.
- **EOxCloudless:** The **2016 mosaic** is distributed under **CC BY 4.0**; the **2018–2025 mosaics** have **CC BY-NC-SA 4.0** terms for non-commercial use. Attribution wording varies by mosaic year. Consult the [EOX license and attribution page](https://cloudless.eox.at/license-non-commercial), and retain visible attribution on maps and published outputs.
- **FABDEM v1.2:** Licensed under **CC BY-NC-SA 4.0**. Credit the dataset creators and the University of Bristol; commercial-use questions should be directed to the dataset rights holders. See the [official FABDEM record](https://research-information.bris.ac.uk/en/datasets/fabdem-v1-2/).
- **Overture Maps:** Licensing and attribution requirements vary by theme and underlying contributor. Some themes include data licensed under **ODbL**. Review the [official Overture attribution requirements](https://docs.overturemaps.org/attribution/).
- **Mapterhorn, Esri, Google Maps, OpenStreetMap, and other online services:** Follow the individual providers' service terms, attribution rules, and any restrictions on imagery extraction, caching, redistribution, or derived products.
- **AI models, libraries, and datasets:** Retain their separate licenses, notices, and attribution obligations, including those applicable to model weights or training datasets.

EarthMapper does not transfer ownership or usage rights in third-party imagery, data, models, or services. The application's availability at no cost does not automatically make all uses of those resources non-commercial.

## Platform

- **Windows desktop application** built with .NET / WPF.
- Requires **Microsoft Edge WebView2 Runtime** for map display.
- Some basemaps, historical imagery, satellite imagery, downloads, terrain, and elevation services require an internet connection.
- Locally imported datasets and supported editing, analysis, and GeoAI workflows can operate without a continuous internet connection.
- GeoAI inference can run locally using the included ONNX model.

## Feedback

Bug reports, suggestions, and feature requests are welcome through the [EarthMapper GitHub repository](https://github.com/AliAlkazraji/EarthMapper).

---

**EarthMapper — Practical mapping, surveying, satellite imagery, terrain, GeoAI, and geospatial analysis in one free desktop application.**
