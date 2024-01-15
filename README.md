## NYC Electricity Demand Prediction
* Please download htmls to view
### Summary
* Predicting demand (load forecasting) is a fundamental activity for grid operators and electricity market participants. Accurate load forecasts help in planning and scheduling generation and transmission resources effectively.
* This project evaluates the performance of 24-hour electricity load forecasting machine learning (ML) models for NYC using weather variables.
* (for detailed EDA and data preprocessing see NYC_EDA_preprocessing.html)

#### Aim:
* Build ML models capable of 24-hour ahead load forecasting with potential real-world application.
* Choose variables for the models which would likely be available to forecasters 24-hours in advance i.e. given the accuracy of 24-hour ahead weather forecasts, weather forecast variables are considered acceptable.
* Evaluate ML model performance.

#### Models:
* Baseline: decision tree (DT), linear regression (LR)
* Advanced models: linear regression (LR) and XGBoost with tree-based boosting (xgboost)
* (Models were chosen according to literature review of most popular ML models in similar projects)

#### Data:
* Hourly, 2016 - 2019
* Independent variables:
    * Weather = dry-bulb temperature, precipitation, humidity, pressure
    * Time/date = month, hour
    * Engineered Features:
      * 24hr lag = all weather features, MWh
    * Weekday/weekend
* Dependent variable:
    * Electricity demand (MWh)
