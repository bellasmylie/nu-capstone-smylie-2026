# nu-capstone-smylie-2026
Predicting Automotive Powertrain Demand Trends
A Data-Driven Analysis of EV, Hybrid, and ICE Vehicle Adoption

Project Overview

The automotive industry is undergoing a major transformation as electric vehicles (EVs), hybrid vehicles, and alternative powertrains reshape the future of transportation. Manufacturers must make long-term strategic decisions about where to invest, often without complete certainty about future demand.

This project uses data analysis and predictive modeling to evaluate historical trends and forecast future demand across powertrain types.

Goal: Provide data-driven insights to help automotive manufacturers determine whether to prioritize EVs, hybrids, or internal combustion engine (ICE) vehicles.

Research Question

Should automotive manufacturers prioritize electric vehicles, hybrids, or internal combustion engines based on demand trends and predictive modeling and in which region?

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

Removed missing values
Converted date fields to datetime
Extracted time features (year, month)
Standardized column formats

Feature Engineering

Feature Engineering

The following features were created to improve model performance:

revenue_per_unit → pricing efficiency
demand_growth → demand trends over time
lag_sales → previous demand (time-based feature)
Brand_Code → encoded categorical variable
Region_ variables* → one-hot encoded geographic indicators

Modeling Approach

Multiple models were used to analyze and predict demand trends:

Two models were used to analyze EV demand:

Linear Regression
- Baseline model
- Easy to interpret
- Used for comparison
Random Forest Regression
- Captures non-linear relationships
- Provides feature importance
- Best performing model

Model Comparison

Models were evaluated using:

R² (Coefficient of Determination)
MAE (Mean Absolute Error)

Key Findings
EV Demand Drivers (Model Results)
Battery capacity strongly influences demand
Discounts and pricing impact sales
Regional differences affect adoption
Demand follows non-linear patterns


Limitations
Limited historical data in BTS dataset
Potential bias in Kaggle dataset
Lack of real-time consumer preference data
Simplified feature engineering

Clone this repository
- Navigate to the /notebooks/ folder
- Run all cells from top to bottom
- Data is located in /data/
- Final results appear in the last section of the notebook
