# Cybercrime Analysis: A Longitudinal Data-Driven Study (2015-2024)

Pavan Kumar Masters Project | Coventry University

## Overview

This project presents a reproducible quantitative analysis of cybercrime trends in the United States over a ten-year period from 2015 to 2024. Using data sourced from FBI Internet Crime Complaint Center (IC3) Annual Reports, the study examines how cybercrime has evolved structurally, financially, and demographically. The analysis covers 39 crime types across ten years and applies multiple analytical methods to extract policy-relevant insights.

## Research Objectives

- Identify long-term trends in cybercrime complaint volumes and financial losses
- Quantify the structural shift in the cybercrime landscape before and after 2020
- Cluster cybercrime types by behavioural patterns using unsupervised learning
- Analyse demographic victimisation patterns across age groups
- Build predictive models to forecast future complaint volumes and financial losses

## Dataset

- Source: FBI Internet Crime Complaint Center (IC3) Annual Reports, 2015 to 2024
- Coverage: 39 cybercrime types over 10 years
- Format: Manually compiled and harmonised panel dataset
- Note: Automated PDF extraction was not feasible due to inconsistent report formatting; data was compiled and cleaned manually to ensure accuracy and consistency

## Methodology

The analysis is structured into five interrelated stages:

1. Exploratory Data Analysis: Distribution of complaint volumes and financial losses across crime types and years
2. Trend and Growth Rate Analysis: Year-on-year changes and cumulative growth across the study period
3. K-Means Clustering: Grouping of 39 crime types into structurally distinct clusters based on complaint and loss patterns
4. Demographic Analysis: Examination of age-group victimisation rates, with a focus on the 60+ population
5. Predictive Modelling: ARIMA for time-series forecasting of complaint volumes; Random Forest Regressor for predicting complaints and financial losses

## Key Results

- Average annual financial losses rose from approximately 2.44 billion before 2020 to 10.41 billion after 2020, representing a 327 percent increase
- Investment fraud accounted for 6.57 billion in losses in 2024; Business Email Compromise (BEC/EAC) accounted for 2.77 billion
- K-Means clustering identified three structurally distinct groups of cybercrime types, confirming that different crime categories follow different developmental trajectories
- The 60+ age group consistently accounted for the highest share of financial losses, ranging from 28.58 to 41.82 percent across the study period
- ARIMA forecasts predict a plateau in complaint volumes between 651,000 in 2025 and 2027
- The Random Forest model achieved an R-squared of 0.91 for complaint prediction and 0.70 for loss prediction on the held-out test set

## Repository Structure

```
cybercrime-analysis/
|-- notebook/          # Jupyter notebook containing all analysis and visualisations
|-- data/              # Compiled panel dataset (CSV format)
|-- report/            # Final project report (PDF)
|-- README.md          # Project overview
```

## Tools and Technologies

- Python 3
- pandas, NumPy
- matplotlib, seaborn
- scikit-learn (K-Means, Random Forest)
- statsmodels (ARIMA)
- Jupyter Notebook

## How to Run

1. Clone this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn statsmodels`
3. Open the notebook inside the `notebook/` folder using Jupyter Notebook or JupyterLab
4. Run all cells in order

## Reference

FBI Internet Crime Complaint Center (IC3). (2024). Internet Crime Report 2024. Federal Bureau of Investigation.
