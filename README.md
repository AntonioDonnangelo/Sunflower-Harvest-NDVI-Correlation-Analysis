# Sunflower-Harvest-NDVI-Correlation-Analysis
Generate spatially interpolated data (IDW) of a series of parameters analyzed in field (e.g. Yield), and correlate them with the average Normalized Difference Vegetation Index (NDVI) over the previous year

## Key Features and Components:

The input data is a geopackage file representing a set of points. Each point has a series of characteristics, such as: georeferenced coordinates (Longitudine, Latitudine), product weight (RESAKG), harvester speed (VELOCITA), harvested area (AREA), and product humidity (UMIDITA).    

Visual rappresentation of the points:  

![field_points](images_readme/field_points.png)

### Data Cleansing and Preparation: 
The repository includes scripts and guidelines for preprocessing raw yield data.   
This involves handling missing values, remove duplicates and other operations. 
Steps for cleaning and formatting data ensure accuracy and consistency for subsequent analyses.  
An exploration of key underlying statistics is also done.

The first lines of the geopackage::

![data_head](images_readme/data_head.png)

### Spatial Interpolation: 
Spatial interpolation techniques are implemented to interpolate yield data across the field.   
Algorithms such as Inverse Distance Weighting (IDW) are utilized to generate continuous yield maps from discrete data points.  
Explanations and implementations of these algorithms are provided, along with examples of input data formats and output data formats (raster maps).

Spatially interpolated data (Yield):

![yield_idw](images_readme/yield_idw.png)

NDVI mean:

![NDVI](images_readme/NDVI_mean.png)

### Correlation with NDVI: 
At the end, harvested yield and humidity are correlated with NDVI (Normalized Difference Vegetation Index) calculated over the sunflower coltivation year (march-september) for the same field.   
This correlation provides insights into how yield variations relate to vegetation health indicators.  

Plot of the correlation between yield and the average NDVI:

![resa_ndvi_corr](images_readme/resa_ndvi_corr.png)

### Extra: Generate a vector file for field application
Once the interpolated yield or vigor data are obtained, it is possible to convert this information into vector format for the application of precision farming operations.

![shape_yield](images_readme/shape_3classes.png)