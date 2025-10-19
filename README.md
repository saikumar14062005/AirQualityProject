# Air Quality Prediction Project

## Overview
Machine Learning project using UCI Air Quality Dataset to predict pollutant concentrations and classify air quality levels.

## Dataset
- Records: 9,357 hourly measurements
- Features:
  1. `Date` – Monitoring date
  2. `Time` – Monitoring hour
  3. `CO(GT)` – True hourly averaged CO concentration (mg/m³)
  4. `PT08.S1(CO)` – CO-sensitive sensor response
  5. `NMHC(GT)` – True hourly averaged Non-Methane Hydrocarbons (µg/m³)
  6. `C6H6(GT)` – True hourly averaged Benzene concentration (µg/m³)
  7. `PT08.S2(NMHC)` – NMHC-sensitive sensor response
  8. `NOx(GT)` – True hourly averaged Nitrogen Oxides concentration (ppb)
  9. `PT08.S3(NOx)` – NOx-sensitive sensor response
  10. `NO2(GT)` – True hourly averaged Nitrogen Dioxide concentration (µg/m³)
  11. `PT08.S4(NO2)` – NO2-sensitive sensor response
  12. `PT08.S5(O3)` – Ozone-sensitive sensor response
  13. `T` – Ambient temperature (°C)
  14. `RH` – Relative Humidity (%)
  15. `AH` – Absolute Humidity
  16. `hour` – Extracted hour from datetime
  17. `dayofweek` – Extracted day of the week
  18. `month` – Extracted month

- Source: [UCI Air Quality Dataset](https://archive.ics.uci.edu/dataset/360/air+quality)

## Project Tasks
1. Exploratory Data Analysis (EDA)  
   - Study pollutant trends hourly, daily, weekly, and seasonally
   - Analyze relationships between pollutants, sensor responses, and weather conditions
2. Regression Models: Linear Regression, Decision Tree Regressor, Random Forest Regressor  
   - Predict pollutant concentrations (e.g., CO(GT), NOx(GT), C6H6(GT))  
3. Classification Models: Logistic Regression, Decision Tree Classifier, Random Forest Classifier  
   - Predict air quality categories (e.g., Good, Moderate, Unhealthy)  
4. Model Comparison with hyperparameter tuning  
   - Compare performance using RMSE, MAE, R² for regression  
   - Compare performance using Accuracy, Precision, Recall, F1-score for classification

## How to Run
1. Open `airQuality.ipynb` in Jupyter Notebook  
2. Install required packages:
   ```bash
   pip install pandas scikit-learn matplotlib seaborn numpy
