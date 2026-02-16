# A Bayesian Data Fusion Model of Temperature in Norway Using the INLA-SPDE Method

This repository contains the R code developed for the master’s thesis **_A Bayesian Data Fusion Model of Temperature in Norway Using the INLA-SPDE Method_**.

It includes:
- The full code used to build and estimate the final models  
- Supporting scripts for data preparation and processing  
- Selected plots and intermediate methods used in model development

A link to the published thesis will be added here once it becomes available: [Link to thesis](#)

# Abstract

Meteorological data in Norway comes from both weather stations and numerical models. Each of these data sources have their own limitations: spatial coverage of observations are often sparse, while forecasts can be biased. To improve the quality of temperature information in Norway, it may be useful to combine these data sources within a single statistical model. This thesis explores a Bayesian data fusion approach using the INLA–SPDE method. The numerical forecast dataset is derived from NORA3, a downscaling of ERA5, while the observations of daily mean temperature come from Frost API, MET Norway’s archive of historical weather and climate data.

# About this repository

A substantial part of the project is devoted to data preparation and preprocessing. To maintain clarity and avoid overwhelming the methodological components, all data preparation scripts and helper functions are organised in a separate folder: [`data_preparation/`](./data_preparation)

Most plots were created using `ggplot2` following consistent plotting principles, with only minor variations depending on the data type. To avoid redundancy, not all plotting scripts are included. The plots that are directly relevant to the thesis results can be found in: [`plots/`](./plots)

The core model implementation, including mesh construction, SPDE specification, and INLA model fitting, is located in: [`models/`](./models)

The final fitted models used to produce the thesis results are stored in: [`final_models/`](./final_models)
