# 6. Spatial Autocorrelation
In this section we used the open source GeoDa software to measure spatial autocorrelation and map clusters, using global and local Moran's I tests.

## Maps Produced

![]()

## Dataset Used 

1. Election_2021.shp -Kartverket, downloaded from geonorge.no
2. Election statistics - Valgdirektoratet, downloaded from valgresultat.no

## Discussion
The GeoDa software was used to conduct the spatial autocorrelation test (Global and Local Moran's I test) on Norway's election data. QGIS was used to symoblise the LISA map.
 
1. Global Moran's I test 
K-nearest neighbours = 6 was used to define the neighbourhood relationship for the test.
Univariate Moran's I test was conducted on percentage of votes to the Labour party. 
The value was found to be 0.519, with a p value < 0.05, showing a positive and significant correlation between neighbourhood municipalities voring for the Labour party. 

2. Local Moran's I test
A LISA map (Local Indicators of Spatial Association) was prepared to identify clusters in voting patterns. 
The Univariate Local Moran's I test was run on the data for percentage of votes to the labout party and the map was imported to QGIS.
A High-High correlation was found in the regions of Finnmark, Innlandet and some parts of Trøndelag.