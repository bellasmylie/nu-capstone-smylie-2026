# nu-capstone-smylie-2026
Predicting Automotive Powertrain Demand Trends
A Data-Driven Analysis of EV, Hybrid, and ICE Vehicle Adoption

Project Overview

The automotive industry is undergoing a major transformation as electric vehicles (EVs), hybrid vehicles, and alternative powertrains reshape the future of transportation. Manufacturers must make long-term strategic decisions about where to invest, often without complete certainty about future demand.

This project uses data analysis and predictive modeling to evaluate historical trends and forecast future demand across powertrain types.

Goal: Provide data-driven insights to help automotive manufacturers determine whether to prioritize EVs, hybrids, or internal combustion engine (ICE) vehicles.

Research Question

Should automotive manufacturers prioritize electric vehicles, hybrids, or internal combustion engines based on demand trends and predictive modeling?

Repository Structure
/data/
    bts_vehicle_sales.csv
    ev_adoption_kaggle.csv

/notebooks/
    1_data_preparation.ipynb
    2_exploration.ipynb
    3_modeling.ipynb
    4_model_comparison.ipynb

/results/
    figures/
    model_outputs/

README.md
Data Sources
1. U.S. Bureau of Transportation Statistics (BTS)
Source: https://www.bts.gov/content/gasoline-hybrid-and-electric-vehicle-sales
Key variables:
Year
Hybrid vehicle sales
Electric vehicle sales
Gasoline vehicle trends
2. Kaggle EV Adoption Dataset
Source: https://www.kaggle.com/datasets/rameezmeerasahib/electric-vehicle-ev-sales-and-adoption
Key variables:
Year
Location/demographics
Vehicle type
Sales volume
Data Preparation

To ensure accuracy and consistency, the following steps were performed:

Identified and removed missing values (.dropna())
Converted columns to appropriate numeric formats
Checked for duplicates and inconsistencies
Standardized datasets for modeling
Feature Engineering

New variables were created to improve analysis:

numeric_total → total demand across vehicle types
numeric_avg → average demand across variables
high_flag → binary indicator (high vs. low demand based on median)

These features simplified comparisons and improved model performance.

Modeling Approach

Multiple models were used to analyze and predict demand trends:

🔹 Linear Regression (Baseline)
Simple, interpretable model
Used as a benchmark
🔹 Logistic Growth Model
Captures EV adoption curves
Models acceleration and saturation behavior
🔹 Prophet Time Series Model
Forecasts future demand
Handles trend and time-based patterns
🔹 Random Forest Regression
Captures non-linear relationships
Identifies key drivers of EV demand

Model Comparison

Models were evaluated using:

R² (Coefficient of Determination)
MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)

Key Findings
EV adoption is consistently increasing
Growth is non-linear and accelerating
Hybrid vehicles act as a transition technology
ICE vehicles are expected to decline over time
Overall demand remains stable but is shifting toward electrification


Real-World Implications
For Automotive Manufacturers:
Increase investment in EV development
Use hybrids as a short-term transition strategy
Gradually reduce reliance on ICE vehicles

For Industry Operations:
Shift supply chains toward EV components
Retrain workforce for EV systems
Adapt dealership service models

Limitations
Limited historical data in BTS dataset
Potential bias in Kaggle dataset
Lack of real-time consumer preference data
Simplified feature engineering

Future Work
Incorporate pricing, fuel cost, and incentives
Add consumer sentiment analysis
Expand to global datasets
Apply advanced machine learning models

Clone this repository
- Navigate to the /notebooks/ folder
- Run all cells from top to bottom
- Data is located in /data/
- Final results appear in the last section of the notebook
