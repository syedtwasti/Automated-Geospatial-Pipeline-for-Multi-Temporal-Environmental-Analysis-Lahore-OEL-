🌍 Automated Geospatial Pipeline for Multi-Temporal Environmental Analysis (Lahore District)

An end-to-end, fully automated geospatial analytics pipeline for monitoring environmental change using multi-temporal NASA HLS Sentinel-2 imagery. The system processes vegetation and water indices, performs zonal statistical analysis, and generates district-level insights without manual GIS intervention.

🔗 Repository:
https://github.com/syedtwasti/Automated-Geospatial-Pipeline-for-Multi-Temporal-Environmental-Analysis-Lahore-OEL-/tree/main

📌 Project Overview

This project implements a complete geospatial data engineering workflow for Lahore District, Punjab, Pakistan, using multi-temporal remote sensing data from NASA AppEEARS. It focuses on environmental monitoring through spectral indices and spatial aggregation at administrative levels.

The pipeline transforms raw satellite imagery into actionable insights through:

Automated data ingestion
Raster preprocessing & compositing
Vegetation/water index computation
Zonal statistical analysis
Comparative temporal visualization
🛰️ Study Area & Time Period
Location: Lahore District, Punjab, Pakistan
Time Period: July–September (2023 vs 2024)
Spatial Unit: Tehsil-level administrative boundaries
📡 Data Source
NASA AppEEARS
HLS Sentinel-2 Surface Reflectance (30m)
Product: HLSS30.VI.020
🧪 Spectral Indices Used
NDVI (Normalized Difference Vegetation Index)
NDWI (Normalized Difference Water Index)
SAVI (Soil Adjusted Vegetation Index)
EVI (Enhanced Vegetation Index)
⚙️ Pipeline Architecture
1. Data Ingestion
Automated file discovery from Google Drive
Regex-based metadata extraction (DOY, index, year)
2. Preprocessing
Fill value masking (-28672)
Radiometric scaling (0.0001 factor)
Shape harmonization for raster stacking
3. Composite Generation
Pixel-wise temporal averaging
Multi-scene aggregation per index/year
4. Spatial Analysis
Zonal statistics using tehsil boundaries
Mean index extraction per administrative unit
5. Visualization
Multi-panel comparison maps (2023 vs 2024 vs change)
District boundary overlays
Color-coded environmental classification
📊 Key Outputs
Multi-index raster composites (2023 & 2024)
Tehsil-level environmental summary table
Temporal change detection maps
CSV export of zonal statistics
📈 Example Insights
Vegetation patterns remain spatially stable across study years
Agricultural zones show consistently higher NDVI/EVI values
Urban core exhibits low vegetation and low moisture signals
Water distribution is primarily canal-driven and spatially constrained
⚠️ Known Limitations
CRS inconsistency across raster sources may affect spatial precision
Some QA outputs indicate potential raster validity issues
No advanced interpolation or uncertainty quantification applied
Heuristic thresholds used for change classification
Raster alignment is assumed rather than fully enforced
🚀 Future Improvements
Integration of STAC-compliant data pipelines
Automated workflow orchestration (Airflow / Prefect)
Multi-district scaling for regional analysis
Machine learning-based anomaly detection
Population + urban pressure overlay analysis
Cloud deployment for real-time monitoring
🛠️ Tech Stack
Python (GeoPandas, Rasterio, NumPy, Pandas)
Rasterstats
Matplotlib
Google Colab
NASA AppEEARS API Data
Shapefile-based GIS processing
📁 Repository Structure
data/
  raw/
    2023/
    2024/
  shapefiles/

outputs/
  composites/
  maps/
  reports/

notebooks/
  main_pipeline.ipynb
👨‍💻 Author

Syed Tuaha Wasti
Geospatial Engineering & Data Science

📜 License

This project is intended for academic and research use.
