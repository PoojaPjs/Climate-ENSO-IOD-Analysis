# Climate-ENSO-IOD-Analysis (1998 - 2019) 
This repository contains the full workflow, datasets (where allowed), and Python scripts used to analyze 20+ years of climate variability in relation to major ocean–atmosphere indices, focusing on:

1. ENSO (El Niño–Southern Oscillation)

2. IOD (Indian Ocean Dipole)

3. Rainfall variability across India and Southeast Asia

The study covers the period 1998–2019, using multiple statistical and visualization approaches to understand the relationship between large-scale climate oscillations and monsoon precipitation.

## Project Overview
This project investigates how ENSO and IOD influence rainfall variability across six key regions:

1. North India

2. Central India

3. South India

4. Thailand

5. Indonesia

6. Malaysia

Using Python-based analysis, the study evaluates: Monthly rainfall variations, Seasonal precipitation patterns, Anomaly detection & smoothing, Pearson correlations with ENSO (MEI.v2) and IOD (DMI) indices, EOF (Empirical Orthogonal Function) analysis for dominant climate modes. 

All rainfall data were processed as spatial averages, aggregated by region and month for the full 22-year period.

## Methodology Summary
-1. Data Preparation

   -* Extracted monthly rainfall datasets (1998–2019) for all six regions

   -* Computed spatial means for each region

   -* Created monthly rainfall anomalies

   -* Applied smoothing (Rolling / LOESS) for noise reduction

2. ENSO & IOD Index Processing

   -* Used MEI.v2 for ENSO

   -* Used DMI (Dipole Mode Index) for IOD

Cleaned, melted, and merged monthly index data with rainfall anomalies

Seasonal groupings: DJF, MAM, JJA, SON

3. Statistical Analysis

Pearson correlation between ENSO/IOD indices and rainfall anomalies

Both monthly and seasonal correlation matrices were generated

Seasonal correlations saved as individual CSV files

4. Visualization

Time-series plots of monthly rainfall

Monthly anomaly plots

Seasonal and annual rainfall variability

Bar plots of ENSO–rainfall and IOD–rainfall correlations

Scatter plots and heatmaps (where applicable)

5. EOF Analysis

Performed EOF decomposition to identify dominant spatial patterns

Visualized principal components and explained variance

## Tools & Libraries Used

This project relies on:

Python 3.10+

Pandas

NumPy

Matplotlib

Xarray

Cartopy (if mapping EOFs)

SciPy

scikit-learn (for EOF/PCA)

## 📈 Key Outputs

The repository includes:

Correlation Coefficient CSVs

ENSO vs rainfall (monthly & seasonal)

IOD vs rainfall (monthly & seasonal)

Climate Plots

Monthly rainfall time series

Rainfall anomalies

Smoothed anomalies

Correlation bar charts

EOF spatial & temporal patterns

## 🎯 Objectives of the Study

The main research questions:

How does ENSO influence rainfall across India and Southeast Asia?

Does IOD contribute significantly to rainfall variability in each region?

Which regions show the strongest ENSO/IOD teleconnections?

What dominant modes of rainfall variability are revealed by EOF analysis?

How do monthly and seasonal dynamics differ?

## 📜 Citation

If you use this repository or code, please cite:

Author: Pooja Priya Jeynathi Sethumathavan 
Project: Climate–ENSO–IOD Analysis (1998–2019)
Year: 2024
