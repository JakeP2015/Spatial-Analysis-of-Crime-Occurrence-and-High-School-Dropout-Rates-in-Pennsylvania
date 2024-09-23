# Spatial-Analysis-of-Crime-Occurrence-and-High-School-Dropout-Rates-in-Pennsylvania
1.define study area
   
2 gather data
-   crime rate data from PA uniform crime reporting system (ucr.pa.gov)
-   high school dropout data (education.pa.gov)
-   shapefile of pa counties
- aggregated values from 2021 to 2022

3. convert to same spatial resolution
- crime was at county level
- dropout was at school level and aggregated to county level

4. join data with counties shapefile in ArcGIS Pro
   
5. create spatially lagged variable by generating contiguity-based spatial weight table in GeoDA
   
6. generae local morans i scatter plot, lisa cluster map, and lisa significance map (one for each crime and dropout)
   
7. visually interpret results
