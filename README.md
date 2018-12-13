# Spatial-Data-Mining

## Methods:

The main goal of this project is to analyze Canadian tweets over geographic data to detect any regional variations in word usage. The main libraries used for this task are the following: 
- Geopandas - supports datatypes to handle geospatial data 
- Pysal - spatial analysis functions (Local Getis-Ord G*)

As Tobler’s first law of geography states, “Everything is related to everything else, but near things are more related than distant things.” This project explores spatial autocorrelation to understand how similar closer objects are to other nearby objects.

## Compute Local Getis-Ord G* for select terms 

The Local Getis-Ord G* algorithm allows us to analyze hot spots by calculating the Z-score which is used to determine where features with high or low values cluster spatially. The algorithm analyzes each feature within the context of neighboring features. Positive Z-scores indicate clustering of high values (hot spots colored red) whereas negative z-scores indicate clustering of low values (cold spots colored blue).

## Compute Local Getis-Ord G* for all words then compute PCA 

The Local Getis-Ord G* was computed for all words in the dataset, then Principal Component Analysis was computed to find the top 3 principal components that capture the most amount of variation in terms. 


