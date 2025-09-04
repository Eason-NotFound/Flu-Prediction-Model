# Flu-Prediction-Model
Influenza forecasting model tailored for Hong Kong: Utilising daily border crossings, atmospheric temperature, air quality, and historical clinic attendance figures to predict future influenza trends.
## Model
In our analysis, we sequentially tested random forests, ANNs, and XGBoost, but all performed poorly. Ultimately, we discovered that a lag existed between patient consultation times and influenza outbreaks. Consequently, we incorporated temporal factors into the XGBoost model, resulting in a significantly improved performance.
## Data
All data sourced from https://data.gov.hk/en/
