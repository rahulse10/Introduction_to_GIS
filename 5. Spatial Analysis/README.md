# 5. Spatial Autocorrelation
In this section we explored spatial autocorrelation using global Moran's I and map clusters using local Moran's I. pen source software GeoDa and Qgis was used for this exercise.

## Maps Produced

![LISA map]

##Dataset Used 

1. Water bodies (innsjo and elv) and Administrative boundaries(hamar_admin) - Noregs vassdrags- og energidirektorat (NVE)
2. Elevation information (hamar_hoyde) - Kartverket
3. Buildings (hamar_buildings) - OpenStreetMap, extracted using geofabrik.de
4. Population statistics(population250) - Statistisk sentralbyrå (SSB)


##Discussion
Hamar is located in Innlandet county and is one of the most flood vulnerable places in Norway. 
To create the flood vulnerability map, First a buffer of 150 m around the water bodies (Lakes and Rivers) was created using the **Buffer** and **Merge** tool. 
Secondly, areas of low elevation (under 130m) were identified using the **Definition Query**. Then using the Feature to Polygon tool, the area under Hamar municipality was split between high and low elevation.
Then the vulnerability map was created by identifying areas that are near the water bodies and have a low elevation. The **Clip** tool was used to identify the areas that fall under both categories.
Then the **Feature to Point** tool was used to identify buildings and total number of residents living in the flood risk area. The count was 315, and was found using **Summarize within** tool.
