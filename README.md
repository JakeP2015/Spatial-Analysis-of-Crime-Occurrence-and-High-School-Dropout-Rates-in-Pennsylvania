# Spatial-Analysis-of-Crime-Occurrence-and-High-School-Dropout-Rates-in-Pennsylvania

Spatial autocorrelation for both total crime and high school dropout counts for Pennsylvania at the county level with a temporal resolution of 2021 to 2022 

<h2>Description</h2>
This analysis will use the state of Pennsylvania as a case study from the years 2021 to 2022. The main research questions that this analysis aims to answer are, 1. What counties contain the highest rates of crimes, 2. What counties have the highest rates of high school dropout rates, and 3. How does the spatial autocorrelation of each variable compare? The purpose of these questions is to determine the counties that contain the highest crime and dropout rates at the county level and measure the spatial autocorrelation in order to produce a result of the most promising counties for high school graduation. The premise of this study is to properly inform young adults and their parents of the risks that their area has on crime and high school dropout rates to present them with the best opportunity to be successful in life. 
<br />
<br />
A simple observation of the dataset used for this analysis which is outlined in table 1 indicates that there are similarities between the crime and dropout data for the year 2021 to 2022. The top five counties with the highest rates of crime are Philadelphia, Allegheny, Montgomery, Delaware, and Bucks. The top five counties with the highest rates of high school dropouts are Philadelphia, Dauphin, Allegheny, Chester, and Berks. Applying this dataset to a choropleth map gives a visual representation of where extreme values are located.
<br />
<br />
This analysis is supported even further by measuring spatial autocorrelation using a univariate Local Moran’s I tool in the software Geoda. Once spatial autocorrelation was measured, it was determined that both variables examined in this analysis (crime rate per county and high school dropout rate per county), displayed similar results. Both variables exhibit positive spatial autocorrelation. Moran’s I value for crime was calculated to be 0.166 and high school dropout was 0.106. The supporting cluster maps indicated that both have two prominent clusters. The northern end of Pennsylvania presents a cluster that is associated with low-low values and the southeastern cluster is associated with high-high values meaning that counties with high rates of crime and high school dropouts are surrounded by similar counties. LISA significance maps also corroborate this analysis by indicating that significant events in the dataset are also located in the same general clusters. Counties that have high rates of crime and high school dropouts (southeastern area of Pennsylvania) and also demonstrate positive spatial autocorrelation include Delaware, Philadelphia, Montgomery, and Bucks. Some of the safest counties in this dataset that have low rates of crime and high school dropouts as well as exhibiting positive spatial autocorrelation include Mckean, Potter, Lycoming, Clinton, Cameron, Elk, Forest, Clarion, and Jefferson.
<br />
<br />
One of the limitations of this dataset is the spatial resolution. The coarsest resolution available was at the county level because crime rate would not go any lower. The finest resolution for high school dropout rates was at the singular school level. Therefore, the preciseness of this measurement was severely limited. 

<br />


<h2>Software Used</h2>

- <b>ArcGIS Pro</b> 
- <b>GeoDA</b>
- <b>Microsoft Excel</b> 

<h2>Analysis walk-through:</h2>

<p align="center">
Define study area: <br/>
<img src="" height="80%" width="80%" />
<br />
<br />
Gather data:  <br/>
<img src="" height="80%" width="80%" />
<img src="" height="80%" width="80%" />
<br />
<br />
Convert to same spatial resolution: <br/>
<img src="" height="80%" width="80%" />
<br />
<br />
Join data with counties shapefile in ArcGIS Pro <br/>
 <img src="" height="80%" width="80%" />
<br />
<br />
Create spatially lagged variable by generating contiguity-based spatial weight table in GeoDA:  <br/>
<img src="" height="80%" width="80%" />
<br />
<br />
Generate Local Moran's I scatterplot, LISA Cluster Map, and LISA Significance Map:  <br/>
<img src="" height="80%" width="80%" />
<br />
<br />
Visually Interpret Results <br/>
<img src="" height="80%" width="80%" />
<br />
<br />

</p>
