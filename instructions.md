# instructions
##  instructions - updated 18 April 2024
Excellent work has been done so far. Few points:

- Link to the online data files [available here](https://github.com/IsamAljawarneh/datasets/tree/master/data) instead of the local files, so that I can run directly!
- test with larger datasets, same data but more records, available [here](https://github.com/IsamAljawarneh/datasets/tree/master/data/NYC_AQ) for the AQ data.
- Start writing your paper!
    - I will add reference papers later on. Focus now on discussing the results that you have obtained and drawing an architectural overview of the framework, we can discuss those points in a meeting.

----------------------------------------------------------
1. [ ] run the example starting code and familiarize yourself with some geosaptial processing techniques, including:
    - sampling
    - spatial join
    - geo-visualization

2. [ ] reference papers include:
    > [1. joining mobility and Air Quality data](https://www.mdpi.com/1999-5903/15/8/263) 

3. [ ] Your task is to develop a novel algorithm based on dimensionality reduction (geohash, Google's S2 or Uber's H3) and filter-and-refinement approach of spatial join, to join mobility data (e.g., taxi trajectory data) with low-cost air quality data (e.g., snensor readings measuring particulate matters PM10 and PM2.5), then you develop a framework for the exploratory data analytics of the combined data, including but not limited to teh following:
- geo-visualization of the data. For example, generating heatmaps and coropleth thematic maps (a.k.a. aggregation-based thematic geomaps)
- Generating graphs to study the autocorrelation in the data, such as histograms.
- Exploratory Spatial Data Analysis (ESDA) [example](https://darribas.org/gds_scipy16/ipynb_md/04_esda.html), such as ```Spatial Autocorrelation```
- Exploratory Spatial and Temporal Data Analysis (ESTDA), [example](https://darribas.org/gds_scipy16/ipynb_md/05_spatial_dynamics.html), such as ```Spaghetti Plot```, ```Kernel Density (univariate, aspatial)```, ```Markov Chains```, and ```Spatial Markov```, [Spatial Autocorellation](https://github.com/PacktPublishing/Geospatial-Data-Science-Quick-Start-Guide/blob/master/Chapter04/Chapter4.ipynb), and [GLobal Spatial Autocorrelation](https://github.com/PacktPublishing/Geospatial-Data-Science-Quick-Start-Guide/blob/master/Chapter04/Chapter4.ipynb) 

- formulating and testing hypothesis on the integrated views of the data. For example, Null hypothesis: have taxi mobility been less near the NYC city center, the air quality would be better (in terms of less pollution PM10 and PM2.5 levels), any discripancy is due to chance only. Alternative hypothesis: differences are not due to chance, there is another factor.

    > get insights from the following:
    - [02_geovisualization](https://darribas.org/gds_scipy16/ipynb_md/02_geovisualization.html)
    - [Exploratory Spatial Data Analysis (ESDA)](https://darribas.org/gds_scipy16/ipynb_md/04_esda.html)
    - [NYC Data](https://github.com/PacktPublishing/Geospatial-Data-Science-Quick-Start-Guide/blob/master/Chapter02/NYC%20Data.ipynb)
    - [Performing Spatial operations like a Pro](https://github.com/PacktPublishing/Geospatial-Data-Science-Quick-Start-Guide/blob/master/Chapter03/Chapter3.ipynb) such as ```Spatial join```
    
    ---------------
    
    NEW!! 31 March 2024
    - you need to proceed by applying the concepts we have covered in the last few chapters (visualization, sampling, testing hypothesis, mean, prediction, classification) to the fused (merged) data that results from joining air quality and mobility data.
    - for example (for testing hypothesis chapter), formulate hypothesis about the ratio between the average PM25 value at a specific neighborhood and the density of taxi fleet moving at the same time in that neighborhood. Have a look at HW2 for more insights.
    - for example (for sampling chapter), design a novel stratified-like sample method that take samples fairly from each neighborhood (probably by sampling from each geohash bracket the same value) based on the distribution of PM25 and taxi trip values, from the combined dataset that results from the join. Then quantify uncertainty by measuring, for example Root-Mean-Square (RMSE) error between the predicted PM10/density ratio value (which results from the sampling) and the original value from the original dataset without sampling.  
    - for example (for mean chapter), apply the concepts that we have studied on ```choosing sample size```, ```properties of the mean```, ```variability```, ```SD and normal curve```, ```central limit theorem``` and ```variability of the sample mean``` on one of the statistics, which is the ```mean of pm25```
    - for example (for prediction chapter), apply the regression to check wether we can predict the pm10 value in a specific location (could be represented as a geohash) given the density of taxi at that location at the same time!
    - I also have added the conference (and journal) paper template to start writing your report!