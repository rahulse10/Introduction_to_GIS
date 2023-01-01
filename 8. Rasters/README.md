# 8. Rasters
In this section we learned about raster data, satellite imagery and tools used to extract informations from it.

## Maps Produced

![](https://github.com/rahulse10/Introduction_to_GIS/blob/main/5.%20Spatial%20Analysis/Layout.jpg)

## Dataset Used 

1. dtm10.tif - Geodata AS / Statens Kartverk, downloaded from hoydedata.no
2. roads_osm_bergentettsted.shp - OpenStreetMap, extracted using geofabrik.de
3. buildings_osm_bergentettsted.shp - OpenStreetMap, extracted using geofabrik.de
4. N50_water_bergen.shp - Kartverket, downloaded from geonorge.no
5. sentinel2_bergen2020.tif - Copernicus Sentinel-2 / Kartverket / CESBIO – CNES, downloaded from geonorge.no

## Discussion
5 maps were produced using different Raster function tools. /
1. A hillshade map was prepared for Bergen. It is a grayscale represntation of the shades produced when sunbeams hit the surface. /
2. Aspect map of Bergen which tells us about the cardinal direction of a slope. Using the Add Surface Information tool, the information derived from the Aspect map was addedd to the buildings dataset of the region. 
This can be used to check the orientation of the ground on which each building stands. /
3. Slope map of Bergen was prepared with the DTM . Using the Add Surface Information tool, the information derived from the Slope map was addedd to the roads dataset of the region.
This can be used to check the slope of the roads which can be used to predict what roads will people most likely use to walk. /
4. A Contour map was prepared with contour interval of 50m.
5. For the last map, green area in Bergen were identified using Normalized difference vegetation index (NDVI) function. Using Sentinel 2 staellite image and Green NVDI imagery tools, the map was prepared. 
Finally, Green Areas were symoblised using the **Reclassify** Tool. 