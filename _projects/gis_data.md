---
layout: page
title: GIS Data Visualization 
description:
img: assets/img/qgis_apple.png
importance: 5
category: project
---


## 🗺️ GIS Data Visualization Projects

This collection of GIS projects showcases how spatial data—such as satellite imagery, elevation models, and hazard frequency maps—can be processed and visualized to inform environmental analysis and real-world decision-making.

---

### 📍 Using ArcGIS

#### 🔥 Sea Surface Temperature Analysis with MODIS Satellite Data

- **Objective**: Track sea surface temperature (SST) variations after the Hunga Tonga–Hunga Haʻapai volcanic eruption in 2022  
- **Data Source**: NASA MODIS satellite imagery  
- **Tool**: ArcGIS Pro  
- **Insights**: Visualized temperature changes in the ocean, revealing environmental impacts of volcanic ash and its effects on marine ecosystems

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/arcgis_sst_1.PNG" title="MODIS SST Analysis" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/arcgis_sst_2.PNG" title="MODIS SST Visualization" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

### 🌿 Using QGIS

#### 🍎 Suitability Mapping for Apple Cultivation

- **Goal**: Identify optimal apple farming zones based on geospatial conditions such as slope, rainfall, and temperature  
- **Approach**: Layered GIS data to score each region’s agricultural suitability  
- **Impact**: Assists farmers in site selection and reveals how climate change is shifting suitable cultivation zones

#### 🥾 Hiking Trail Planning in Jirisan

- **Goal**: Design safe and accessible hiking trails by referencing locations of shelters, KTX train stations, and bus terminals  
- **Tools**: Used QGIS for spatial routing and 3D visualization  
- **Use Case**: Supports outdoor safety and enables quick-response planning for emergencies like wildfires or rescue missions

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/qgis_apple.png" title="Apple Suitability Map" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/qgis_hiking.png" title="Jirisan Hiking Route Map" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

#### 🌧️ Optimal Evacuation Mapping During Floods

- **Focus**: Analyze flood- and landslide-prone zones, assess transportation accessibility, and recommend alternative evacuation routes  
- **Result**: Generated detour paths and emergency access corridors from high-risk areas to shelters  
- **Application**: Can enhance disaster management planning and support smart city safety infrastructure

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/qgis_flood_bus.png" title="Bus-Based Evacuation Routes" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/qgis_flood_taxi.png" title="Taxi Network for Emergency Travel" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

---

### 🧭 Technology Stack Summary

| Domain               | Tools & Techniques                               |
|----------------------|--------------------------------------------------|
| Satellite Image Analysis | ArcGIS Pro, MODIS Satellite Data               |
| Spatial Analysis & Mapping | QGIS, DEMs, Soil/Climate Layers                |
| 3D Visualization     | QGIS 3D Viewer    |
| Disaster Response Planning | QGIS Network Analysis, Raster Statistics, Evacuation Routing |

---
