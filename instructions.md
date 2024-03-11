# instructions
## follow the following instructions
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
- Exploratory Spatial and Temporal Data Analysis (ESTDA), [example](https://darribas.org/gds_scipy16/ipynb_md/05_spatial_dynamics.html), such as ```Spaghetti Plot```, ```Kernel Density (univariate, aspatial)```, ```Markov Chains```, and ```Spatial Markov```

- formulating and testing hypothesis on the integrated views of the data. For example, Null hypothesis: have taxi mobility been less near the NYC city center, the air quality would be better (in terms of less pollution PM10 and PM2.5 levels), any discripancy is due to chance only. Alternative hypothesis: differences are not due to chance, there is another factor.

    > get insights from the following:
    - [02_geovisualization](https://darribas.org/gds_scipy16/ipynb_md/02_geovisualization.html)
    - [Exploratory Spatial Data Analysis (ESDA)](https://darribas.org/gds_scipy16/ipynb_md/04_esda.html)