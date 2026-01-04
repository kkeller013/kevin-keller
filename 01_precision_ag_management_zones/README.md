# Precision Viticulture: Management Zone Delineation  
**Calistoga AVA, Napa Valley**

## Project Overview
This project applies multi-layer spatial analysis and unsupervised clustering to delineate vineyard management zones within the Calistoga AVA. By integrating vegetation, soil, and topographic variables, the analysis identifies spatially distinct production zones to support site-specific irrigation, canopy management, and drainage decisions.

**Key Outcome:**  
A four-zone management framework was developed that explains statistically significant differences in vine vigor and site conditions, enabling targeted vineyard interventions rather than uniform management.

---

## Management Zone Map (Overview)
![Management Zones Map](maps/Calistoga_MZ_clip.jpg)

*A four-zone K-means clustering result integrating NDVI, slope, clay percentage, and aspect.*

---

## Problem Statement
Vineyards within the Calistoga AVA exhibit substantial spatial variability in vigor, soil composition, and terrain. Managing these areas uniformly can lead to inefficient irrigation, inconsistent vine growth, and suboptimal fruit quality. This project asks:

**How can spatially explicit data be used to delineate vineyard management zones that support precision viticulture decisions?**

---

## Approach

### Data & Inputs
- **Vegetation:** NDVI (Landsat 8 OLI/TIRS)
- **Topography:** Slope and aspect (SRTM DEM)
- **Soils:** Clay percentage
- **Spatial Framework:** 200 m × 200 m fishnet grid

### Methods
1. Extracted NDVI, slope, aspect, and clay percentage values to a uniform grid.
2. Standardized variables to ensure equal weighting in clustering.
3. Determined the optimal number of clusters using the Elbow Method (k = 4).
4. Applied K-means clustering to delineate management zones.
5. Validated cluster separation using ANOVA (NDVI differences significant at p < 0.001).
6. Mapped and interpreted management zones within ArcGIS Pro.

### Tools
- **GIS & Remote Sensing:** ArcGIS Pro, Landsat 8, SRTM DEM  
- **Data Analysis:** R (tidyverse, cluster, factoextra)  
- **Precision Ag Concepts:** Spatial variability analysis, management zone delineation

---

## Results

### Spatial Patterns by Variable
![NDVI by Cluster](maps/CalistogaNDVI_clip.jpg)
![Clay % by Cluster](maps/CalistogaClayPct_Clip.jpg)
![Aspect by Cluster](maps/CalistogaAspect_clip.jpg)
![Slope by Cluster](maps/CalistogaSlope_Clip.jpg)

### Cluster Summary

| Cluster | NDVI  | Clay % | Slope (°) | Aspect | Management Interpretation |
|------|------|--------|----------|--------|---------------------------|
| **1** | 0.287 | 14.3 | 16.3 | W–SW | Steep slopes → erosion control and irrigation uniformity |
| **2** | 0.306 | 13.7 | 14.7 | N–NE | High vigor → canopy management priority |
| **3** | 0.224 | 20.8 | 3.56 | E–SE | Low vigor; clay-heavy → drainage improvement needed |
| **4** | 0.261 | 51.6 | 8.55 | N–NE | Balanced conditions → moderate, targeted inputs |

---

## Insights & Recommendations
- Vine vigor varies systematically with slope, aspect, and soil texture rather than randomly across the landscape.
- Clay-rich, low-slope areas consistently exhibit reduced NDVI, indicating potential drainage and root-zone constraints.
- High-vigor zones benefit from canopy management to balance vegetative growth and fruit quality.
- Management zones enable targeted interventions, reducing input waste while improving consistency and resilience.

---
## Limitations & Future Work
- The analysis relies on remotely sensed NDVI as a proxy for vine vigor and does not incorporate measured yield or fruit quality data.
- Spatial resolution is constrained by satellite imagery; higher-resolution drone-based imagery could improve zone delineation accuracy.
- Incorporating in-field soil measurements would strengthen validation of the soil texture layer and improve confidence in zone interpretation.
