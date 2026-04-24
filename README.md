# Automated-Geospatial-Pipeline-for-Multi-Temporal-Environmental-Analysis-Islamabad-OEL-
A fully automated Python-based geospatial processing pipeline for multi-temporal environmental monitoring of Islamabad using satellite-derived indices. The project computes zonal statistics for administrative boundaries and performs temporal change detection for vegetation and water stress using open-source GIS libraries in Google Colab.

🌍 Project Overview

This project implements an end-to-end automated GIS workflow for environmental monitoring of Islamabad. It processes satellite-derived indices (NDVI, NDWI, EVI, SAVI) across two time periods to analyze vegetation health and surface water dynamics at the administrative (Tehsil/Union Council) level.

The pipeline is built using Python in Google Colab and focuses on reproducibility, scalability, and automation of traditional GIS workflows.

⚙️ Key Features
Automated loading of multi-temporal raster datasets
Zonal statistics computation for administrative boundaries
Temporal change detection (environmental trend analysis)
Generation of derived raster outputs (change maps)
Export of GIS-ready GeoJSON outputs with attributes
Thematic visualization of spatial patterns
🧠 Technologies Used
Python
Rasterio
GeoPandas
Rasterstats
NumPy
Matplotlib
Google Colab

Satellite data sourced from:

NASA AppEEARS
📊 Workflow Summary
Load satellite-derived raster indices (NDVI, NDWI, EVI, SAVI)
Preprocess and clean raster datasets
Align raster and vector coordinate reference systems (CRS)
Compute zonal statistics for administrative units
Perform temporal change detection across two time periods
Generate raster and vector outputs
Visualize spatial patterns using thematic maps
📁 Outputs Generated
GeoTIFF raster outputs (e.g., NDVI change raster)
GeoJSON file with appended zonal statistics
Thematic maps (vegetation and water stress analysis)
📌 Key Insight

This project demonstrates how traditional manual GIS workflows can be transformed into a fully automated geospatial analytics pipeline, enabling faster and more scalable environmental monitoring for decision-making.

🚀 Future Improvements
Integration with real-time satellite APIs
Web-based GIS dashboard deployment
Machine learning-based environmental prediction models
Population-environment correlation analysis
