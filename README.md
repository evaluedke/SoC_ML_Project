# SoC_ML_Project
# Arctic Sea Ice Prediction with ERA5 Climate Dara

## Description 

## Data 
The data for this project is a global reanalysis ERA5 dataset with monthly data from 1981-2023 (https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels-monthly-means?tab=overview, https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-pressure-levels-monthly-means?tab=overview). In a previous process a new dataset has been selected, in which specific variables at required pressure levels and at ground level have been combined and only a selected region (north of 50°N) has been chosen. The dataset can be found on zenodo (16.75GB) under the following link: 10.5281/zenodo.13387782

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

The code is structured into several sections. In the beginning, there is a preprocessing part in which the data 
