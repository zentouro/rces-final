## Drought variables across CMIP6 | RCES Final Project 2020 


<!-- [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zentouro/rces-final/main) --> <!-- Regular Binde -->

[![Binder](https://binder.pangeo.io/badge_logo.svg)](https://binder.pangeo.io/v2/gh/zentouro/rces-final/main) <!-- Pangeo Binder -->

[More information on this project and class](https://earth-env-data-science.github.io/projects.html)


-----------------
#### Research Question
What is the relationship between drought-associated variables across CMIP6 Model Experiments?


----
#### Data Sets
This project queries model experiments from the [Sixth phase of the Coupled Model Intercomparison Project (CMIP6)](https://www.wcrp-climate.org/wgcm-cmip/wgcm-cmip6). As these datasets can be quite large, they will be accessed through google cloud storage managed by [Pangeo](https://pangeo-data.github.io/pangeo-cmip6-cloud/). 

Variables of interest:
- tasmax - max temperature (A)
- tas - temperature (A)
- smsos - soil moisture (L)


____
#### Hypothesis 
Drought-associated variables, like max temperature, temperature, and soil mositure will be highly correlated, but there will be significant spread across model experiments. 


-------
#### Analyses
The `final_project.ipynb` notebook uses the package `intake-esm` to query and load model experiments that include all three of the variables of interest. This could easily be adjusted for other variables used across CMIP6. 

After masking the loaded model experiments across land, I plot all queried models to visually compare spread for various experiments. I also calculated and plot a spatial pearsons correlation for two of the model experiments. 

The second half of the notebook loads the entire time series for the same models, variables, and experiments, reduced to global annual mean and combined into a single large dataset. This is then plotted over the entire model run for visual analysis of climate change-related drends.  

#### Future Work

This notebook could be expanded to include cross-correlation for all queried model experiments. There are also several other drougt-associated variables in CMIP6 that could be incorporated.


