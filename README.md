# Zillow Price Analysis
A data-driven analysis of historical housing prices to forecast future trends and identify top-performing ZIP codes for investment opportunities.

## Project Overview
This project uses **time series models** (ARIMA, SARIMAX, and Prophet) to analyze and forecast housing prices for various ZIP codes.  
The primary goal is to identify ZIP codes with the **highest forecasted growth** to guide investment decisions.

The analysis includes:
- Historical price trends.
- Forecasting future values using ARIMA, SARIMAX, and Prophet models.
- Visualizing growth across top ZIP codes.

## Dataset
- **Source**: Zillow housing price dataset.
- **Description**: Contains historical housing prices for different ZIP codes, including:
   - `Time`: Date of observation.
   - `Value`: Average housing price.
   - `Zip_Code`: ZIP code identifier.
- **Time Range**: 1996 - 2018.
- **Frequency**: Monthly.

## Workflow
1. **Data Cleaning and Preparation**:
   - Removed missing values and outliers.
   - Resampled data to a monthly frequency.
2. **Exploratory Data Analysis (EDA)**:
   - Visualized trends and seasonal patterns in housing prices.
3. **Modeling**:
   - Used **ARIMA** and **SARIMAX** for time series forecasting.
   - Implemented **Prophet** to capture trends and seasonality.
4. **Forecast and Results**:
   - Forecasted housing prices for the next 12 months.
   - Identified ZIP codes with the highest forecasted growth.
5. **Visualization**:
   - Plotted growth trends and bar charts for the top 5 ZIP codes.

## Model Results

We applied multiple time series models to analyze and forecast housing prices across ZIP codes. Below are the key results:

Models Compared:
1. ARIMA(1,1,1):
AIC: 4321.540, BIC: 4332.268
Captures trends and recent changes effectively.
2. ARIMA(2,1,1):
AIC: 4338.381, BIC: 4352.684
Added complexity with no significant improvement.
3. SARIMAX(2,1,1)x(1,1,1,12) (Best Performing Model):
AIC: 3063.263, BIC: 3084.096
Accounts for seasonality (12-month cycles) and delivers the best fit.
4. Prophet Model:
RMSE: 4944.39, MAE: 4693.55, R²: 0.21
Struggles to explain variability in the data.

## Next Steps
Deep Dive into Top ZIP Codes:

Conduct additional analysis of demographics, economic trends, and housing demand in the identified regions.
Incorporate External Features:

Integrate economic indicators (e.g., job growth, income levels) to enhance the SARIMAX model.
Automate and Monitor:

Develop a pipeline to regularly update forecasts as new data becomes available.
Visualize Insights:

Build an interactive dashboard for stakeholders to explore forecasts and trends dynamically.
Explore Advanced Models:

## Navigating the Git Repository 
1. [ReadME](https://github.com/alecs1523/zip_code_investment_analysis/blob/main/README.md)
2. [CAGR_zip_code_csv](https://github.com/alecs1523/zip_code_investment_analysis/blob/main/forecasted_growth_results.csv)
3. [zillow data](https://github.com/alecs1523/zip_code_investment_analysis/blob/main/zillow_data.csv)
4. [Presentation PDF](https://github.com/alecs1523/zip_code_investment_analysis/blob/main/zip_code_investment_analysis.pdf)
5. [Jupyter Notebook](https://github.com/alecs1523/zip_code_investment_analysis/blob/main/zip_code_price_predictions.ipynb)



## Contact
**Alec Schonfeld**  
Email: alecschonfeld15@gmail.com
GitHub: https://github.com/alecs1523
