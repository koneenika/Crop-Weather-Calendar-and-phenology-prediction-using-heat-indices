🌾 Crop Weather Calendar & Prediction of Phenology Using Heat Indices

This project predicts wheat phenological stages (from emergence to maturity) using heat indices such as Growing Degree Days (GDD) and temperature-based features.
By integrating multi-year weather data (2019–2024) with machine learning models, the project generates a data-driven crop growth calendar that can assist in agricultural monitoring, planning, and forecasting.

🧠 Project Overview

The goal of this project is to analyze and predict wheat growth stages based on accumulated heat units.
It automates the workflow of:

Extracting stage-wise phenological data from a Word file.

Processing daily weather data from Excel.

Computing GDD (Growing Degree Days) and temperature statistics.

Training and evaluating multiple ML models to predict stage timing.

⚙️ Features

Converts phenology tables into a clean, usable format.

Calculates GDD and cumulative temperature indices.

Trains ML models — Linear Regression, Random Forest, SVM, and XGBoost.

Generates prediction tables and model performance metrics (MSE, RMSE, MAE, R²).

Produces comparative visualizations for model evaluation.


🧩 Methodology

Data Extraction:

Reads phenological stage data from a Word document.

Reads daily max/min temperature data from Excel.

Feature Engineering:

Calculates daily and cumulative GDD using a base temperature of 5°C.

Derives average temperature per stage.

Model Training:

Models trained: LinearRegression, RandomForestRegressor, SVR, XGBRegressor.

Features: CumGDD_to_stage, AvgTemp_to_stage.

Target: DaysFromSowing.

Evaluation Metrics:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

Coefficient of Determination (R²)

✅ Best Model: Random Forest (R² = 0.89)

🧰 Tech Stack

Languages: Python

Libraries: pandas, numpy, sklearn, xgboost, python-docx, matplotlib

Tools: Jupyter Notebook, Google Colab, Excel


📈 Future Enhancements

Integrate soil moisture and NDVI data for improved accuracy.

Automate visualization of phenology calendars.

Extend model generalization to other crops and agro-climatic zones.

