# Fishing Effort Spatial Analytics  
**Participation, Access, and Pressure Across Eastern U.S. Coastal States**

## Project Overview
This project analyzes recreational fishing activity across Eastern U.S. coastal states mapping total fishing effort over a 15 year period, then breaking down that effort through spatial normalization methods. By examining fishing trips (effort) relative to population, coastline length, and fishing mode, the analysis demonstrates how different spatial lenses fundamentally change the interpretation of fishing participation and pressure.

**Key Insight:**  
Observed fishing effort reflects a combination of participation intensity, physical access, and behavioral preference; normalizing by population and coastline reveals patterns that are obscured in raw totals.

---

## Analytical Question
Recreational fishing activity varies widely across coastal states, but total fishing effort alone does not explain why activity is high in some areas and lower in others. This analysis explores the structural drivers of fishing effort by examining how population size, shoreline availability, and fishing behavior contribute to observed spatial patterns.

---

## Approach

### Data
- Recreational fishing trips by state and fishing mode
- State population (year-matched)
- Coastline length by state (proxy for shoreline access)
- U.S. state boundaries for spatial mapping

### Methods
1. Aggregated fishing trips to the state level.
2. Calculated total fishing effort as a baseline metric.
3. Normalized fishing effort by population (trips per capita) to reflect participation intensity.
4. Normalized fishing effort by coastline length (trips per km) to reflect access-constrained pressure.
5. Calculated fishing mode shares (%) to provide behavioral context.
6. Visualized spatial patterns using choropleth maps and supplemented results with a bivariate scatterplot.

### Tools
- ArcGIS Pro (joins, normalization, mapping)
- Spreadsheet analysis for QA and summary statistics

---

## Results

### 1. Total Fishing Effort (Observed Outcome)
**What this shows:**  
Where the largest absolute volumes of fishing activity occur.

![Placeholder: Total Fishing Effort Map](maps/total_fishing_effort_placeholder.png)

*Total fishing trips by state. High values reflect combined effects of population size, access, and fishing culture.*

---

### 2. Fishing Effort per Capita (Participation Intensity)
**What this shows:**  
Where fishing participation is disproportionately high relative to population size.

![Placeholder: Fishing Effort per Capita Map](maps/fishing_effort_per_capita_placeholder.png)

*Trips per capita highlight states where fishing represents a stronger cultural or recreational activity.*

---

### 3. Fishing Effort per Kilometer of Coastline (Access-Constrained Pressure)
**What this shows:**  
Where fishing activity is concentrated along limited shoreline access.

![Placeholder: Fishing Effort per Coastline Map](maps/fishing_effort_per_coastline_placeholder.png)

*Trips per km of coastline reveal states where physical access constraints may intensify fishing pressure.*

---

### 4. Fishing Mode Context (Behavioral Structure)
**What this shows:**  
How fishing activity is distributed across shore, private boat, and charter modes.

![Placeholder: Fishing Mode Share Map](maps/fishing_mode_share_placeholder.png)

*Fishing mode shares provide context for interpreting shoreline pressure and participation patterns.*

---

### 5. Participation vs Access Interaction (Supplemental Analysis)
**What this shows:**  
The relationship between reliance on shore fishing and access-constrained fishing pressure.

![Placeholder: Scatterplot – % Shore Fishing vs Trips per km Coastline](outputs/scatter_shore_vs_coastline_placeholder.png)

*States with higher reliance on shore fishing often exhibit elevated fishing effort per kilometer of coastline, suggesting an interaction between access-dependent fishing modes and spatial concentration of effort.*

---

## Interpretation
- Total fishing effort reflects multiple structural drivers and can obscure localized pressure.
- Per-capita normalization highlights participation intensity and fishing culture independent of population size.
- Coastline-normalized effort captures access constraints and spatial concentration of activity.
- Fishing mode share helps explain why similar effort levels can imply very different access and pressure dynamics across states.

Together, these perspectives demonstrate that fishi

