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

This was performed using **Climate Data Operators (CDO)** in a Linux environment.

Example command:

```bash
cdo remapbil,gridfile input.nc output.nc
