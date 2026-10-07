# EarthMapper

**EarthMapper** is a free Windows desktop mapping application for viewing, creating, editing, analyzing, and exporting geospatial data in a simple and practical environment.

It is designed for users who need common GIS and surveying tools without requiring a full GIS package for every task.

## Key Features

- **2D and 3D mapping** with online and offline workflows.
- Import and work with **KML/KMZ, Shapefile (SHP), DXF, CSV, GeoTIFF**, and other common geospatial data.
- Export vector data to formats such as **KML/KMZ, SHP, DXF, and CSV**.
- Export maps as **PNG, JPEG, TIFF, and GeoTIFF**.
- Draw and edit **points, lines, polygons, rectangles, squares, circles, and ellipses**.
- Precise drawing using **Distance, Direction/Azimuth, Distance + Direction, Angle, and ΔX/ΔY** constraints.
- **Identify, Select, Move, Split, Buffer, Measure, Snap, Undo**, and geometry editing tools.
- **Line Division** by equal parts or specified segment length, with optional division points.
- **Area Division** for fixed-size parcels, equal-area parcels, and equal-width divisions.
- Coordinate support for **WGS 84 Geographic, UTM, and MGRS**.
- Custom **Geographic, UTM, and MGRS grids**, including manual spacing and advanced grid-point labeling.
- **Elevation profiles, point elevations, DEM generation, contours, and 3D terrain** using multiple elevation sources.
- Create profiles from **lines or point layers**, with distance, stationing, or point-number X-axis modes.
- Compare up to **three elevation sources** in one profile with source-difference statistics.
- Generate **DEM and contour lines** from Mapterhorn elevation data or user point layers using **IDW or Kriging**.
- **GeoAI object detection** on imported GeoTIFF imagery using a built-in aerial OBB model or a custom ONNX model.
- Native-resolution tiled GeoAI processing with class selection, overlap handling, progress display, and georeferenced detection output.
- **Esri Wayback historical imagery** support.
- Shapefile CRS detection and supported reprojection during import.
- Advanced layer styling, labeling, attribute viewing, feature-level styling, and project saving.
- Multi-feature summaries with geometry statistics, extents, detailed reports, and HTML export.

## Free to Use

EarthMapper is **free to use**.

The application itself is provided free of charge. Third-party libraries, map providers, elevation services, AI models, and online data sources used by EarthMapper remain subject to their own licenses, attribution requirements, usage limits, and terms of service.

## Acknowledgements

EarthMapper is built with and makes use of several excellent open-source projects, frameworks, datasets, and online mapping services.

Special thanks to:

- [Leaflet](https://leafletjs.com/) — interactive 2D web mapping.
- [MapLibre GL JS](https://maplibre.org/) — 3D map/globe rendering and terrain visualization.
- [Mapterhorn](https://www.mapterhorn.com/) — online DEM terrain and elevation data used for terrain, elevation profiles, and elevation sampling.
- [Esri](https://www.esri.com/) — World Imagery, Topographic basemaps, and Wayback historical imagery services.
- [OpenStreetMap](https://www.openstreetmap.org/) contributors — OpenStreetMap basemap data.
- [Google Maps Platform](https://mapsplatform.google.com/) — optional Google map and imagery services.
- [Microsoft WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) — integration of the web mapping engine inside the Windows desktop application.
- [NetTopologySuite](https://github.com/NetTopologySuite/NetTopologySuite) — geometry processing and spatial operations.
- [netDxf](https://github.com/haplokuon/netDxf) — DXF reading and writing support.
- Microsoft **.NET / WPF** — desktop application framework used by EarthMapper.
- [Microsoft ONNX Runtime](https://onnxruntime.ai/) — local neural-network inference used by EarthMapper GeoAI.
- [Ultralytics](https://www.ultralytics.com/) — YOLO object-detection framework and model ecosystem.
- [DOTA Dataset](https://captain-whu.github.io/DOTA/) — aerial imagery object-detection dataset used for training and evaluation of oriented object-detection models.
- [YOLO26-DOTA-v2](https://github.com/JustinVladut/YOLO26-DOTA-v2) by Justin Vladut — source of the built-in aerial-oriented object detection model used by EarthMapper GeoAI.

The built-in GeoAI model supports aerial object detection with oriented bounding boxes and includes classes such as aircraft, ships, storage tanks, vehicles, bridges, harbors, airports, helipads, and other DOTA aerial-object categories.

Thank you to the developers, contributors, researchers, and data providers behind these projects, datasets, models, and services.

## Third-Party Services and Licensing

EarthMapper provides access to several third-party basemap, imagery, terrain, elevation, and AI technologies.

Users are responsible for complying with the license and usage conditions of the corresponding provider.

In particular:

- Online basemap and imagery providers may restrict automated extraction or derivative-data generation.
- Mapterhorn elevation data remains subject to its own service terms.
- Google, Esri, OpenStreetMap, and other providers retain their respective ownership and attribution requirements.
- AI models, frameworks, and datasets retain their respective licenses and usage conditions.

EarthMapper does not transfer ownership of any third-party imagery, data, model, or service to the user.

## Platform

- **Windows desktop application**
- Requires **Microsoft Edge WebView2 Runtime** for map display.
- Some basemaps, historical imagery, terrain, and elevation functions require an internet connection.
- GeoAI inference can run locally using the included ONNX model.

## Feedback

Bug reports, suggestions, and feature requests are welcome through the GitHub repository.

---

**EarthMapper — Simple mapping, drawing, analysis, terrain, GeoAI, and geospatial data tools in one desktop application.**
