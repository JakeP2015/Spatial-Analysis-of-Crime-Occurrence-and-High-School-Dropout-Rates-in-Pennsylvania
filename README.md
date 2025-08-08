# Spatial Analysis of Crime and High School Dropout Rates in Pennsylvania

This project uses spatial statistics to examine the relationship between **county-level crime rates** and **high school dropout rates** in **Pennsylvania (2021–2022)**. The analysis was conducted using **ArcGIS Pro** and **GeoDa**, focusing on spatial autocorrelation and geographic clustering.

---

## 🔍 Project Overview

Statistically, high school dropouts are 3.5 times more likely to be arrested than graduates, and 68% of inmates do not hold a high school diploma. This project investigates whether geographic patterns in crime correlate with high school dropout rates to better inform educators and policymakers.

**Research Questions:**
1. Which counties have the highest crime and dropout rates?
2. Are these variables spatially autocorrelated?
3. Do their spatial patterns overlap?

---

## 🧩 Problem Statement

Understanding the spatial dynamics of education and crime can inform interventions in at-risk communities. By analyzing the spatial relationship between crime and dropout rates, we can identify clusters of concern and opportunity.

---

## 📊 Data Sources

| Dataset | Source | Description |
|--------|--------|-------------|
| Crime Data | [ucr.pa.gov](https://www.ucr.pa.gov) | Total crimes by county (2021–2022) |
| Dropout Data | [education.pa.gov](https://www.education.pa.gov) | Dropouts aggregated from school to county level |
| County Boundaries | [PASDA](https://www.pasda.psu.edu) | Pennsylvania county shapefiles |

---

## 🛠️ Tools & Technologies

- **ArcGIS Pro** – Spatial joins, data processing
- **GeoDa** – Spatial autocorrelation, LISA analysis
- **Excel** – Data aggregation via pivot tables
- **Python (optional)** – Data cleaning automation (future expansion)

---

## 📌 Methodology

1. **Data Aggregation**
   - Crime data manually scraped and totaled by county.
   - Dropout data aggregated using Excel pivot tables.

2. **Data Join & Cleaning**
   - Joined crime/dropout data with county shapefiles in ArcGIS Pro.
   - Exported cleaned shapefile for spatial analysis.

3. **Spatial Analysis in GeoDa**
   - Created Queen contiguity-based spatial weights matrix.
   - Ran **Local Moran’s I** for both variables.
   - Generated:
     - Choropleth Maps
     - Moran's I Scatterplots
     - LISA Cluster Maps
     - LISA Significance Maps

---

## 📈 Results

| Metric | Crime Rate | Dropout Rate |
|--------|------------|--------------|
| **Top Counties** | Philadelphia, Allegheny, Montgomery | Philadelphia, Dauphin, Allegheny |
| **Moran’s I** | 0.166 | 0.106 |
| **Clustering** | High-high clusters in Southeast PA | Similar high-high patterns |

**Key Insights:**
- **Positive spatial autocorrelation** found in both datasets.
- Clusters of high crime and dropout rates aligned in southeastern counties: *Philadelphia, Delaware, Montgomery, Bucks*.
- Low-low clusters (safe and stable counties) included *McKean, Potter, Clinton, Elk, and Clarion*.

---

## 🗺️ Visuals

**Crime Rate Choropleth**  
![Crime Rate Choropleth](https://i.imgur.com/TIwSGPv.jpeg)

**Dropout Rate Choropleth**  
![Dropout Rate Choropleth](https://i.imgur.com/dHhQImR.jpeg)

**Moran’s I Scatterplot for Crime Rate**  
![Moran's I Crime Rate](https://i.imgur.com/LvqYnx5.jpeg)

**Moran's I Scatterplot for High School Dropouts**
![Moran's I High School Dropouts](https://i.imgur.com/i4cAS86.jpeg)

**LISA Cluster & Significance Maps for Crime Rate**  
![LISA Cluster Crime Rate](https://i.imgur.com/uhCirhA.jpeg)
![LISA Significance Crime Rate](https://i.imgur.com/dJaW45U.jpeg)

**LISA Cluster & Significance Maps for High School Dropouts**
![LISA Cluster High School Dropouts](https://i.imgur.com/bQRHKDd.jpeg)
![LISA Significance High School Dropouts](https://i.imgur.com/yjD9TKL.jpeg)
