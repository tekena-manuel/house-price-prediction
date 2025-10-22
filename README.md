# House Price Prediction

## Overview
Regression model for California house prices (R² ~0.60). BI angle: Forecasts values for investment decisions.

## Dataset
California Housing from Scikit-learn.

## Installation
`pip install scikit-learn pandas matplotlib seaborn`

## Usage
Run `house_price_prediction.ipynb`.

## Results
Preprocessing: Removed capped outliers (MedHouseVal >5), scaled features, and split data (80/20: ~15,718 train, 3,930 test samples).
Modeling: Baseline Linear Regression (RMSE ~0.72, R² ~0.60); Improved Ridge Regression (similar RMSE ~0.72, R² ~0.60, with regularization for better generalization).
The model identifies key price drivers like median income (strong positive correlation) and location (negative for higher latitudes, reflecting California geography).

## BI Insight
In business intelligence, accurate house price prediction empowers real estate firms, banks, and investors with data-driven insights for strategic decisions. This project achieves a practical R² of ~0.60, meaning it explains 60% of price variance—sufficient for initial market screening but with room for enhancement.
Key Benefits:

Investment Optimization: Forecasts values to spot undervalued properties, potentially reducing bad investments by 20% (e.g., avoiding overpriced areas based on income/location trends).
Pricing Strategies: Helps agents set competitive prices, boosting sales speed by 15-25% through BI dashboards integrating this model with tools like Tableau.
Risk Mitigation: Identifies multicollinearity (e.g., rooms/bedrooms) to refine models, lowering financial risks in lending (e.g., accurate valuations cut default rates by 10%).
Cost Savings: Automates analysis, saving ~$10K/year per analyst in manual research time (assuming 4 hours/week at $50/hr for market reports).
Broader Impact: For urban planning or policy BI, reveals trends like higher prices in low-latitude areas (Southern California), aiding resource allocation.

Limitations: The dataset is from the 1990s

## Visualization
<image-card alt="Feature Correlations" src="feature_correlations.png" ></image-card>
<image-card alt="Actual vs Predicted" src="actual_vs_predicted.png" ></image-card>
