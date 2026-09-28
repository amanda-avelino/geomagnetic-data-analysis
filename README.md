# Geomagnetic Data Analysis

Analysis of geomagnetic observations from Brazilian observatories using INTERMAGNET data and IGRF models.

This project focuses on the processing, analysis, and comparison of geomagnetic observations, using data from Brazilian geomagnetic observatories and geomagnetic reference models.

## Project Status

**In development**

The project is currently being developed as part of an academic research project in geomagnetism.

## Data

The project uses geomagnetic observations from Brazilian observatories obtained from the INTERMAGNET database.

The initial analysis focuses on data from the **Vassouras Geomagnetic Observatory (VSS)**, including one-minute geomagnetic measurements from 2015.

The dataset contains the geomagnetic components:

- X
- Y
- Z
- F

The data are processed to handle missing measurements and organize the observations for subsequent analysis.

## Analysis

The analysis begins with the processing and visualization of geomagnetic observations from the Vassouras Geomagnetic Observatory.

The data are organized using Python and Pandas, allowing the geomagnetic components to be analyzed as time series.

The initial analysis includes:

- Data organization and preprocessing.
- Conversion of date and time information.
- Visualization of the X, Y, and Z geomagnetic components.
- Identification and treatment of missing measurements.

### Nighttime Analysis

To reduce the influence of solar-driven variations, the analysis includes geomagnetic measurements collected during nighttime periods.

For each month, nighttime observations between **00:00 and 06:00 UT** are selected and used to calculate monthly averages of the geomagnetic components.

### Geomagnetically Quiet Periods

To further restrict the analysis to relatively quiet geomagnetic conditions, nighttime observations are combined with the **Dst index**.

Measurements with **Dst > -50 nT** are selected, and the corresponding geomagnetic components are used to calculate monthly averages.

### Multi-year Analysis

The analysis was extended to geomagnetic observations from the **Vassouras Observatory between 2015 and 2020**.

The geomagnetic observations were combined with the Dst index, allowing the selection of nighttime measurements under relatively quiet geomagnetic conditions. Monthly averages were then calculated for the analyzed period.

### Comparison with the IGRF Model

The observed geomagnetic field at the Vassouras Observatory was compared with values predicted by the **International Geomagnetic Reference Field (IGRF)**.

The analysis uses the observatory coordinates and calculates the expected geomagnetic field components for the corresponding periods. The differences between the observed and modeled values are then analyzed.

### Extended Vassouras Dataset

The Vassouras geomagnetic dataset was further extended to cover the period from **2015 to 2025**.

The observations were processed using the nighttime and geomagnetically quiet-period criteria. Missing data were also identified and accounted for during the analysis.

### Tatuoca Observatory

The analysis was extended to observations from the **Tatuoca Geomagnetic Observatory (TTB)** for the period from **2018 to 2025**.

The dataset was processed using the same general approach, including the treatment of missing measurements, nighttime selection, and geomagnetically quiet conditions.

Monthly averages were calculated and compared with the **IGRF** model for the Tatuoca observatory.
