# Airbnb Booking Demand Prediction (Boston)
This project predicts Airbnb listing occupancy rates in Boston using machine learning models.
It aims to identify key factors that drive booking demand and provide actionable insights for hosts and platforms.

## Data
- Source: Boston Airbnb Open Data (InsideAirbnb via Kaggle)
- Time period: 2016-09-05 to 2017-09-04
- Files used:
  - calendar.csv (availability, used to compute occupancy rate)
  - listings.csv (price, room type, capacity, host info, location)
  - reviews.csv (review activity)

## Target Variable
Occupancy Rate  
Occupancy = 1 − AVG(availability)

## Methods
- Exploratory Data Analysis (EDA)
- Feature preprocessing with scikit-learn Pipeline
- Models:
  - Linear Regression
  - Support Vector Regressor (RBF)
  - Random Forest
  - Gradient Boosting
  - Stacking Regressor (best performance)

## Results
- Best model: Stacking Regressor
- RMSE ≈ 0.31
- Key findings:
  - Listings with more reviews have higher occupancy
  - Price–occupancy relationship is nonlinear
  - Central Boston neighborhoods show higher demand

## Notebook
https://colab.research.google.com/drive/1l4JTn2MY-gIIkkqc754kZHRBfzOEWc1p?usp=drive_link

### Team member: Kean Zhu, Yihui Tang, Yu-Jiun Zou, Tzu-Jen Chen
