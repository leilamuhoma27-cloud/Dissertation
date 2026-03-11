# Climate Analysis Using CMIP6 Climate Model
## Project Overview

This repository contains scripts and analysis developed during my MSc dissertation at the University of Reading (Walker Institute).  

The study assessed the **historical and future climate suitability of traditional and diversified cash crops** in Masindi District, Uganda using rainfall and temperature projections from **CMIP6 Global Climate Models (GCMs)**.

The crops assessed include:

- Sugarcane
- Cocoa
- Coffee (Arabica and Robusta)
- Vanilla

The analysis evaluated climate suitability using **crop-specific rainfall and temperature thresholds** under historical and future climate scenarios.

---

## Research Objectives

The main objectives of the study were:

- Assess historical climate suitability (1981–2014)
- Analyse future climate projections (2021–2050)
- Compare suitability under different climate scenarios
- Evaluate how climate change may affect crop diversification strategies

Future climate projections were analysed under:

- **SSP2-4.5** (intermediate emissions scenario)
- **SSP5-8.5** (high emissions scenario)

---

## Data Sources

Climate data used in this analysis includes:

- **CMIP6 Global Climate Model datasets**
- Historical climate observations
- **CRU climate dataset** used as a reference for remapping

Variables analysed:

- Rainfall (precipitation)
- Temperature

---

## Methods and Workflow

### 1. Climate Data Extraction

Python scripts were used to extract rainfall and temperature variables from **CMIP6 Global Climate Model datasets**.

Key tasks included:

- Downloading and reading NetCDF climate files
- Extracting variables (precipitation and temperature)
- Organising datasets for further analysis

---

### 2. Climate Model Selection and Quality Control

Models were evaluated based on:

- Data completeness
- Temporal coverage
- Suitability for the study region

Quality checks were performed to ensure consistency of climate data before analysis.

---

### 3. Spatial Remapping

Global climate model outputs were **remapped to match the spatial resolution of the CRU dataset**.
4. Trend Analysis

Trend analysis was performed using R.

The Mann–Kendall trend test was applied to assess long-term trends in:

Rainfall

Temperature

The Mann–Kendall test is commonly used in climate studies because it detects monotonic trends in environmental time series.

5. Climate Suitability Assessment

Crop-specific temperature and rainfall thresholds were used to evaluate climate suitability for:

Sugarcane

Cocoa

Coffee

Vanilla

Suitability conditions were assessed for:

Historical climate

Future projections under SSP2-4.5 and SSP5-8.5 scenarios

Technologies Used

This project integrates multiple tools commonly used in climate and environmental data science.

Programming Languages

Python

R

Linux Shell

Tools and Libraries

Climate Data Operators (CDO)

NetCDF processing tools

Mann–Kendall statistical analysis

Microsoft Excel for supplementary analysis
This was performed using **Climate Data Operators (CDO)** in a Linux environment.

Example command:

```bash
cdo remapbil,gridfile input.nc output.nc
Key Skills Demonstrated

This project demonstrates expertise in:

Climate data analysis

Handling large climate datasets (NetCDF)

CMIP6 climate model analysis

Climate scenario analysis (SSP pathways)

Spatial data remapping

Statistical trend analysis

Environmental data science workflows

Academic Context

MSc Agriculture and Development
University of Reading, United Kingdom
Walker Institute for Climate System Research

Dissertation Title

Assessment of Historical and Future Climate Suitability for Traditional and Diversified Crops in Masindi District, Uganda
