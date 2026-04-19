# Nairobi Retail Sales Forecasting & Demand Optimization

## Project Overview
End-to-end time series forecasting project for a multi-store retail chain in Nairobi using the Kaggle Store Sales dataset (3M+ transaction records).

The goal was to predict daily sales accurately, understand seasonality patterns, and provide actionable recommendations for inventory planning, staffing, and promotions.

## Business Problem
The retail chain faced frequent stockouts on peak days and overstock on slow days. Key questions included:
- What will daily and weekly sales be in the next 30–90 days?
- How do weekends, holidays, and yearly seasonality affect sales?
- How do external factors like oil prices influence sales?

## Key Insights
- **Strong weekly seasonality**: Sales are significantly higher on weekends, especially Sundays.
- **Clear upward long-term trend**: Sales grew steadily from 2013 to 2017.
- **Holiday impact**: Holidays drive higher sales with greater variability.
- **Yearly seasonality**: December is the strongest month due to year-end shopping.

## Methodology
- **Data Preparation**: Merged sales, stores, oil prices, and holidays datasets. Aggregated to daily level.
- **EDA**: Trend analysis, boxplots, and seasonality detection.
- **Decomposition**: Broke down sales into Trend, Seasonal, and Residual components.
- **Modeling**:
  - Prophet model with holidays and oil price as regressors.
  - SARIMA model with exogenous variables for comparison.
- Generated 60–90 day ahead forecasts with uncertainty intervals.

## Technologies Used
- Python, Pandas, Matplotlib, Seaborn
- Prophet, SARIMA (statsmodels)
- Time Series Decomposition & EDA

## Business Recommendations
- Increase inventory and staffing on Fridays, Saturdays, and Sundays.
- Prepare aggressively for December and major holidays.
- Monitor oil price trends as they appear to influence consumer spending.

## Results
Both Prophet and SARIMA models successfully captured the upward trend and strong weekly seasonality. The forecasts can be directly used for better demand planning.

## How to Run
1. Open the notebook `nairobi_retail_sales_forecasting.ipynb`
2. Run all cells

---

**Made with ❤️ for learning and portfolio purposes**

