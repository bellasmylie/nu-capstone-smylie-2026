# nu-capstone-smylie-2026
Automotive Demand and Adoption Analysis & Forecasting

# Project Overview 
This project creates an analysis based on the adoption and demand trends for Electric (EV), Plug-in Hybrid Electric (PHEV), and Hybrid (HEV) powertrains. This analysis uses historical data and predictive modeling techniques that evaluates industry demand patterns. Forecasts were created to determine future growth to support manufacturing resources. 

# Research Question

Which vehicle powertrain—electric, hybrid, or plug-in hybrid—should automotive manufacturers prioritize based on observed demand trends and predictive modeling, and which geographic region presents the greatest opportunity for growth?

# Datasets Used

•	U.S. Bureau of Transportation Statistics Dataset (2010–2023) 

o	Vehicle type sales data: 

o	Electric Vehicles (EV) 

o	Hybrid Electric Vehicles (HEV) 

o Plug-in Hybrid Electric Vehicles (PHEV) 

	https://www.bts.gov/content/gasoline-hybrid-and-electric-vehicle-sales

•	Test/Train Dataset 

o	Revenue and unit sales by region 

o	Used to identify high-performing markets 

o	https://www.kaggle.com/datasets/rameezmeerasahib/electric-vehicle-ev-sales-and-adoption 


# Methodology
### Data Preparation

•	Cleaned and formatted datasets 

•	Converted year to proper format 

•	Sorted data chronologically

#Feature Engineering

•	Created lag variables (lag_1, lag_2) 

•	Calculated growth rates 

•	Generated future target variables

# Models
### Linear Regression (Baseline)

•	Used to model basic relationship between time and sales 

•	Assumes linear growth

### Lag-Based Regression Model

•	Inputs: 

o	Previous year sales 

o	Growth rate 

•	Predicts future demand

### Random Forest

•	Tested for comparison 

•	Limited effectiveness due to small dataset (BTS)

### ARIMA (Primary Model)

•	Time-series forecasting model 

•	Captures trends and temporal patterns 

•	Used to forecast demand through 2030

## Two models were used to analyze EV demand:

### Linear Regression

•	Baseline model

•	Easy to interpret

•	Used for comparison

### Random Forest Regression

•	Captures non-linear relationships

•	Provides feature importance

•	Best performing model


# Key Findings 

•	Electric Vehicle demand is increasing while Plug-in Hybrid and Hybrid vehicles are acting as intermediate solutions with transitional technology

•	North America is the strongest region with the highest revenue and units sold, this is where manufacturers should be pushing more EV sales as it fits demand 

•	Manufacturers should allocate resources and prioritize Electric vehicle powertrains in North America

# Replication  

Step 1: Open notebook folder 

Step 2: Open necessary ipynb file 

Step 3: Run all cells from top to bottom

Raw Data files will be found in (datasets): "BTS Data.csv", "EV Sales (test).csv", " EV Sales (train).csv"

# Limitations
•	Small dataset (BTS Data) limited some predictive models
•	Models provide future values based on captured trends
•	External factors (government, economy, policies, etc.)

