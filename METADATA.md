# BEES3041_MHW_JEsman

30YrExplore.qmd

Dataset: IMOS - SRS - SST - L3S - Single Sensor - 1 day - night time - Australia
Date range: 1992-Mar-21-15:20-UTC to 2023-Jul-27-15:20-UTC
Format: NetCDF
Authors: Josh & Norton
Summary: QMD where the heatwaveR heatwave detection & analysis took place - dataset used spatial SST data timeseries and obtained thresholds 
for event start, event peak, several intensity parameters, etc.
code was repurposed to process data for 3 study zones and produce plots.
Involved use of custom function and loops to average together each SST daily observation.

Chemical.qmd

Dataset: IMOS - combined geochemical parameters (reference stations)
Date range: 15 years
Format: .CSV
Authors: Man Lim
Summary: Separation of combined parameters into depth profiles and data representation. Used to produce our chemical plots.

Chla_analysis_new.qmd

Dataset: IMOS - SRS - MODIS - 01 day - Chlorophyll-a concentration (OC3 model)
Date Range: 15 years
Format: NetCDF
Authors: Jonathan & Olivier
Summary: Appropriated code from physical analysis used for spatial biological analysis - averaging chlorophyll data into timeseries for
processing in plots. 

MapGraphics.qmd

Dataset: NA
Date range: NA
Format: NA
Authors: Man Lim Ho
Summary: Code to produce study area maps.

RefinedPlots.qmd

Dataset: IMOS - combined geochemical parameters (reference stations)
Date range: 15 years
Format: .CSV
Authors: Man Lim
Summary: Same purpose as Chemical.qmd, this time with more detailed plots

anomalies FINAL.qmd

Dataset: IMOS - SRS - SST - L3S - Single Sensor - 1 day - night time - Australia
Date range: 1992-Mar-21-15:20-UTC to 2023-Jul-27-15:20-UTC
Format: NetCDF
Author: Josh
Summary: Code used to produce anomaly maps. Involved creating two dataframes - reference (15y period average) and heatwave. Subtract
one from the other and run with ggplot2 to obtain heatmap of SST anomalies. 

Unit guide:

Physical analyses (Josh & Norton)

SST = Seas Surface temperature in °C
lon = longitude in °E
lat = latitude in °N
time = time in days (since 1990)

Biological analyses (Jonathan & Olivier)

chl_oc3 = chlorophyll-a in g/m3
time = time in days (since 1990)
longitude = longitude in °E
latitude = latitude in °N

Chemical analyses (Man Lim)

SampleTime_Local = time at which sample was measured in Maria Island, Tasmania
latitude = latitude in °N
longitude = longitude in °E
SampleDepth = depth at which sample was take in m
SampleID = sample reference number
Oxygen_umolL = oxygen concentration in umol/L
Nitrate_umolL = nitrate concentration in umol/L
Phosphate_umolL = phosphate concentration in umol/L
Silicate_umolL = silicate concentration in umol/L
