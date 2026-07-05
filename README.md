# River Water Quality Analysis

## Overview
Time-series analysis of upstream and downstream water quality sensor data to assess the impact of a Water Recycling Centre (WRC) on river health. Completed as a self-directed analytical project using data provided by Wessex Water. This project investigates whether effluent discharge from a Water Recycling Centre has a measurable impact on downstream river water quality. Using continuous sonde monitoring data collected at upstream and downstream locations over a 12-week period, the analysis examines six water quality parameters, their temporal patterns, and their relationship with WRC and river flow conditions.

## Key Techniques
- Multi-sheet Excel data import and standardisation across five datasets
- Data quality validation including missing value analysis, out-of-range detection, anomaly removal, and calibration date filtering
- Time-series visualisation with LOESS smoothing across multiple parameters
- Daily cycle analysis to identify diel patterns in dissolved oxygen and pH
- Spearman correlation matrices with significance testing using the Hmisc package
- Paired t-tests for upstream vs downstream parameter comparisons
- Flow band analysis to assess concentration-dependent effluent effects
- Structured conclusion weighing evidence for and against WRC impact

## Key Findings
- Downstream dissolved oxygen is consistently and significantly lower than upstream (mean 58.40% vs 78.08%, p < 0.001), with - the deficit most pronounced during low WRC flow conditions
- pH follows a similar pattern, with downstream values significantly lower than upstream (mean 7.30 vs 7.63)
- A September divergence where upstream conditions improved independently of WRC operations suggests environmental factors also contribute to observed differences
- Effluent spot sampling data was too temporally sparse to correlate meaningfully with high-frequency sonde readings, leaving the mechanistic link uncertain

## Structure

- WaterQuality.qmd — Main analysis file containing all code, visualisations, and interpretation
- data/ — Not included; data was provided by Wessex Water and is not publicly available

## Requirements
- tidyverse
- knitr
- kableExtra
- readxl
- lubridate
- Hmisc
- broom
- report
- corrplot

### Note
Data was provided by Wessex Water and is not included in this repository. The analysis file is self-contained and documents the full methodology and findings.
