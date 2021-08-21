# Shuswap Lake Modelling  

Exploring hydrologic and meteorologic data at Shuswap Lake, British Columbia.  Building recurrent neural network models to predict lake level and temperature.
___

## Regional Overview

Shuswap Lake and the surrounding region sits west of the Rocky Mountains, east of Kamloops, and north of the Okanangan.  The climate varies throughout the region, with colder and snowier winters in the eastern reaches and at higher elevations, while warmer and drier conditions exist further west and at lower elevations.  Shuswap Lake both is a popular tourist destination and provides important habitat for salmon, among other species.  The lake drains into Little Shuswap River connecting to Little Shuswap Lake, and eventually into the South Thompson River which is a major tributary of the Fraser River.  The lake level demonstrates a seasonal cycle, filling in spring and early summer due to snowmelt and precipitation throughout the basin, and draining through to a minimum level during winter.  

___

## Goals

Here we will explore how well features such as lake level and near-surface water temperature can be modelled using recurrent neural networks (RNNs) with meteorological variables as input.
___

## Data

Daily lake level, near-surface water temperature, maximum air temperature, and minimum air temperature are used from [Shuswap Lake Watch](https://www.shuswaplakewatch.com/index.php).  Hourly wind speed (u- and v-components) is downloaded from [ERA5 climate reanalysis](https://www.ecmwf.int/en/forecasts/datasets/reanalysis-datasets/era5) and aggregated to daily temporal resolution.  Data from 2008 - 2020 (inclusive) is used in these examples.

___

## Files

The files are organized in the following way:
* main_shuswap.ipynb: Contains several examples of modelling lake conditions
* ERA5_u_sicamous_2008_2020.py: Used to download the u-component of hourly wind speed from 2008 - 2020 at Sicamous, British Columbia
* ERA5_v_sicamous_2008_2020.py: Used to download the v-component of hourly wind speed from 2008 - 2020 at Sicamous, British Columbia
* Data/
  * shuswap_lake_data.csv: lake level, water temperature, and air temperature data
  * sicamous_u_2008_2020.nc: u-component of hourly wind
  * sicamous_v_2008_2020.nc: v-component of hourly wind

___

![alt text](https://github.com/andersonsam/shuswap_lake_modelling/blob/main/Images/google_maps.png)
![alt text](https://github.com/andersonsam/shuswap_lake_modelling/blob/main/Images/shuswap_topography.png)

