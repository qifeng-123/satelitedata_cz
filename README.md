# This Repository Include 6 Indexes which are common use to estimate crop yields 

- All Index are exported with Java script through Google Earth API, Each File contails Java script code
- These 6 indexes are consolidated into 1 .xlsx file for fuher analysis use 
- Index Scope : form 2019-01-01 to 2025-04-01 with 8 day interval only for the  Czech Republic
- General Information about these 6 Indexes as below table


<div style="width: 100%; overflow-x: auto;">

| Index | Provider | Bands | Unit | Pixel Size | Description | Cadence | Data Cost | Coding & Validation Time | Data Export Time | Importance for Crop Yield Estimation | Google Earth Engine Dataset |
|-------|----------|-------|------|------------|-------------|---------|-----------|--------------------------|------------------|--------------------------------------|-----------------------------|
| NDWI  | Google   | NDWI  | Unitless (Ratio, -1 to 1) | 30 meters | Normalized Difference Water Index | 8 days | Free | 60 minutes | ~5 minutes (Processing needed, often needs cloud masking, corrections) | Measures plant water content and soil moisture. Early water stress detection prevents yield losses. | [Link](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_COMPOSITES_C02_T1_L2_8DAY_NDWI) |
| NDVI  | Google   | NDVI  | Unitless (Ratio, -1 to 1) | 30 meters | Normalized Difference Vegetation Index | 8 days | Free | 60 minutes | ~5 minutes (Processing needed, often needs cloud masking, corrections) | Measures green biomass and vegetation vigor. High NDVI = healthy plants = good yields. Low NDVI = stress or poor crop. | [Link](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_COMPOSITES_C02_T1_L2_8DAY_NDVI) |
| EVI   | Google   | EVI   | Unitless (Ratio, -1 to 1) | 30 meters | Enhanced Vegetation Index | 8 days | Free | 60 minutes | < 1 min | Better than NDVI in dense forests or high biomass crops (like maize); less sensitive to atmospheric effects. Important for mature crop stages. | [Link](https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_COMPOSITES_C02_T1_L2_8DAY_EVI) |
| LAI   | Google   | LAI   | m²/m² (Leaf Area Index) | 500 meters | Leaf Area Index | 8 days | Free | 30 minutes | < 1 min | Measures leaf area per ground area. Tells you how much "leaf machinery" exists for photosynthesis — a key driver for growth and grain filling. | [Link](https://developers.google.com/earth-engine/datasets/catalog/NASA_VIIRS_002_VNP15A2H) |
| FPAR  | NASA LP DAAC at the USGS EROS Center | FPAR  | Fraction (0 to 1) | 500 meters | Fraction of Photosynthetically Active Radiation | 8 days | Free | 30 minutes | < 1 min | Measures how much sunlight plants actually absorb for photosynthesis. Strong link to biomass accumulation and final yield. | [Link](https://developers.google.com/earth-engine/datasets/catalog/NASA_VIIRS_002_VNP15A2H) |
| LST   | NASA LP DAAC at the USGS EROS Center | LST_Day_1km | Celsius (°C) | 1000 meters | Day land surface temperature | 8 days | Free | 60 minutes | < 1 min | Surface temperature shows drought stress. Too hot = water stress = lower yields. Cool fields = healthy irrigated crops. | [Link](https://developers.google.com/earth-engine/datasets/catalog/MODIS_061_MOD11A2) |


</div>
