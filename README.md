## Drought variables across CMIP6 | RCES Final Project 2020 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zentouro/rces-final/main)

[More information on this project and class](https://earth-env-data-science.github.io/projects.html)


-----------------
#### Research Question
What is the relationship between drought-associated variables across CMIP6 Model Experiments?


----
#### Data Sets
This project will use several model experiments that are part of the [Sixth phase of the Coupled Model Intercomparison Project (CMIP6)](https://www.wcrp-climate.org/wgcm-cmip/wgcm-cmip6). As these datasets can be quite large, they will be accessed through google cloud storage managed by [Pangeo](https://pangeo-data.github.io/pangeo-cmip6-cloud/) 

Variables of interest:
- tasmax - max temperature (A)
- tas - temperature (A)
- smsos - soil moisture (L)


____
#### Hypothesis 
Drought-associated variables, like max temperature, temperature, and soil mositure will be highly correlated, but there will be significant spread across model experiments. 


-------
#### Intended Analyses
My plan is to mask the atmospheric variables (tasmax and tas) to only the grid cells that match the land variable (smsos) - and create global plots for visual comparison, as well as plot timeseries to show climate change-related trends in each variable. I'll also calculate the correlations between the variables for a single model, and compare variables across multiple model experiments. 


