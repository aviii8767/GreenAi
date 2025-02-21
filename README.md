# Solar Energy Usage Prediction - README

## Overview
This project involves building a **Machine Learning (ML) model** to predict **solar energy consumption** based on historical energy usage data. The dataset contains information about different Indian states, energy generation, consumption, surplus energy, and battery storage levels.

## Files Included
- **solar_energy_usage_india.csv** → Dataset containing 500 records of solar energy usage, including weekdays, holidays, and energy consumption details.
- **solar_energy_usage_india.py** → Python script for **data preprocessing, cleaning, and model training**.
- **README.txt** → This document describing the project.

## Requirements
To run this project, install the following Python libraries:
```bash
pip install pandas numpy seaborn scikit-learn matplotlib
```

## Steps to Run the Project
1. **Load the dataset**: `solar_energy_usage_india_weekend_holidays.csv`.
2. **Preprocess the data**:
   - Handle missing values.
   - Convert categorical variables (state, day of the week, holiday) into numerical form using Label Encoding.
   - Drop unnecessary columns like `Date`.
3. **Visualize the data**: Plot energy consumption distribution.
4. **Split the dataset**: 80% for training, 20% for testing.
5. **Standardize features**: Normalize input features for better model performance.
6. **Train a Linear Regression Model** to predict energy consumption.
7. **Evaluate Model Performance** using metrics:
   - **Mean Absolute Error (MAE)**
   - **Mean Squared Error (MSE)**
   - **R-squared Score (R²)**

## Running the Prediction
After training, you can predict energy consumption using:
```python
model.predict([[5,3,1,28,15.69,3.25]])
```

## Expected Outcome
- The model predicts **Energy Consumed (kWh)** based on other variables.
- It helps in optimizing solar energy usage by identifying consumption trends.

## Future Improvements
- Try different ML models like **Random Forest** or **XGBoost**.
- Add **weather conditions** (sunlight hours, temperature) as additional features.
- Improve feature engineering for better accuracy.

---
### Author: Balaji Dhakare

