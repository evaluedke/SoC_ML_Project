# SoC_ML_Project
# Arctic Sea Ice Prediction with ERA5 Climate Data

## Description 

## Data 
The data for this project is a global reanalysis ERA5 dataset with monthly data from 1981-2023 (https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=overview, https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-pressure-levels-monthly-means?tab=overview). In a previous process a new dataset has been selected, in which specific variables at required pressure levels and at ground level have been combined and only a selected region (north of 50°N) has been chosen. The dataset can be found on zenodo (combined_era5_1981-2023.nc, 16.75GB) as well as a dataset for the last part of the analysis (z_1000.nc, 798.5MB) under the following link: https://zenodo.org/records/13387783 

## Code 
To run the code, the following packages are required and can be installed with pip or conda install:
- xarray
- pandas
- numpy
- seaborn
- tensorflow
- scipy
- matplotlib
- cartopy
- sklearn
- statsmodels
- eofs
- warnings

The code is structured into several sections. In the beginning, there is a preprocessing part in which the variables are stored in a dictionary, anomalies are created and area weights are calculated. In the exploratory data analysis, the focus lies on finding correlations between the climatic variables with the goal of choosing the most relevant variables for the machine learning part. In that part, a random forest algorithm is applied to predict sea ice, 2 timeseries prediction approaches: a statistical ARIMA model and a neural network LSTM are compared in predicting the progression of sea ice over time. And finally, an EOF analysis produces the Arctic Oscillation (AO) mode of climate variability to eventually find a relationship between the sea ice fraction and the phase of the AO. 

