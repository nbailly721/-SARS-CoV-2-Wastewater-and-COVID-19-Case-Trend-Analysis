                                                  ######COVID-19 Wastewater Surveillance and Case Trend Analysis in Toronto######

**Description**

This project processes and visualizes SARS-CoV-2 wastewater concentration data alongside COVID-19 case counts for the Toronto region. Using R, the workflow cleans, standardizes, and visualizes weekly and daily trends in 2024, enabling comparison between wastewater viral signals and reported infection rates. The analysis helps assess whether wastewater monitoring reflects community transmission trends.

**Workflow Overview**

    1. Data Import and Cleaning (R Script)

Load raw datasets:

cases.xlsx – Weekly COVID-19 case counts

surveillance.xlsx – Daily SARS-CoV-2 wastewater concentrations for GTA

aggregate.csv – Weekly aggregated SARS-CoV-2 concentrations across Ontario

Standardize date formats across datasets.

Filter for 2024 records and relevant geographic areas (Toronto and GTA).

Select relevant columns and remove missing values to ensure clean datasets for downstream analysis.

    2. Data Visualization and Trend Comparison (R Script)

Generate line plots for:

Daily SARS-CoV-2 concentrations in the GTA

Weekly SARS-CoV-2 concentrations in Toronto

Weekly COVID-19 case rates in Toronto

Normalize and combine wastewater and case data for co-trend visualization.

Plot both metrics on the same graph to explore temporal associations.

**Datasets Used**

cases.xlsx – Weekly COVID-19 case counts in Toronto
Source: Public Health Ontario

surveillance.xlsx – Daily SARS-CoV-2 wastewater concentrations for GTA
Source: Public Health Ontario Wastewater Data

aggregate.csv – Weekly aggregated wastewater concentrations across Ontario
Source: Health Infobase Canada

**Packages Used**

R Environment

tidyverse – Data manipulation and plotting

readxl – Excel import

dplyr – Data wrangling

**Key Results**

Daily wastewater sars concentration in gta.png

Normalized Weekly Trends- COVID-19 Cases vs. Wastewater SARS-CoV-2 in Toronto (2024).png

Weekly Average Wastewater SARS-CoV-2 Concentration in Toronto (2024).png

Weekly Reported COVID-19 Cases in Toronto (2024).png

**Files in This Repository**

wastewater_covid_analysis.R – R script for importing, cleaning, filtering, normalizing, and visualizing datasets

**Important Notes**

Wastewater viral concentrations are standardized and log-transformed at the site level. Values should be interpreted as relative indices, not raw viral copies/mL.

Combined trend plots use min-max normalization to compare wastewater signals with case rates.

Focuses on Toronto (2024) to evaluate whether wastewater-based surveillance reflects reported COVID-19 trends.

**Real-World Relevance**

Supports public health surveillance by comparing wastewater viral loads to reported COVID-19 cases.

Enables early detection of infection trends at the community level.

Provides a reproducible workflow for integrating wastewater and epidemiological data.

Can inform pandemic response strategies and public health interventions.
