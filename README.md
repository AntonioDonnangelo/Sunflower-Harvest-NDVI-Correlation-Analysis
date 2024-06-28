# Sunflower-Harvest-NDVI-Correlation-Analysis
Data preparation and interpolation (IDW) to generate yield distribution rasters, and correlate with the average Normalized Difference Vegetation Index (NDVI) over the previous year

## Key Features and Components:

### Data Cleansing and Preparation: 
The repository includes scripts and guidelines for preprocessing raw yield data.   
This involves handling georeferenced coordinates, product weight (RESAKG), harvester speed (VELOCITA), harvested area (AREA), and product humidity (UMIDITA).   
Steps for cleaning and formatting data ensure accuracy and consistency for subsequent analyses.  

### Spatial Interpolation: 
Spatial interpolation techniques are implemented to interpolate yield data across the field.   
Algorithms such as Inverse Distance Weighting (IDW) are utilized to generate continuous yield maps from discrete data points.  
Explanations and implementations of these algorithms are provided, along with examples of input data formats and output data formats (raster maps).

### Correlation with NDVI: 
At the end, harvested yield and humidity are correlated with NDVI (Normalized Difference Vegetation Index) calculated over the sunflower coltivation year for the same field.   
This correlation provides insights into how yield variations relate to vegetation health indicators.  

### Extra: Generate a vector file for field application
Once the interpolated yield or vigor data are obtained, it is possible to convert this information into vector format for the application of precision farming operations.
