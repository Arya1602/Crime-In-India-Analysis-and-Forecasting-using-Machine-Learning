# Crime in India: Analysis and Forecasting using Machine Learning

This project has been created as part of my research internship on Python and Machine Learning, conducted by Anveshan Foundation, Indira Gandhi Delhi Technical University for Women, New Delhi.

## Introduction to Project
This project explores crime trend analysis and forecasting in India using machine learning and time-series techniques. It combines state-level, city-level crime datasets from NCRB and Kaggle to analyze spatial and temporal patterns of crime and predict future crime rates.

The goal is to provide insights that can support policymakers, law enforcement agencies, and urban planners in making proactive and data-driven decisions for public safety.

## Datasets Used
1.	State wise NCRB Dataset (2001–2022)
•	Covers 14 major crime heads across all states/UTs.
•	Found reporting anomalies after 2018 (sudden unrealistic spikes).
•	Hence, this dataset was primarily used for analysis and visualization.

3.	City wise NCRB Dataset (2014–2021)
•	Crime statistics for major Indian metro cities.
•	Enables finer-grained urban crime analysis.

5.	Kaggle “Indian Crimes Dataset” (2020–2024)
•	Rich city-level dataset with daily crime counts.
•	Pre-processed into a monthly time series for forecasting.

## Methodology
1)	Preprocessing:
•	Aggregated and normalized data to account for population differences.
•	Handled missing values via forward-filling.
•	Converted dates into time-series format for modelling.

2)	Models Applied:
•	Machine Learning Predictors: Decision Tree Regressor, Random Forest Regressor, K-Nearest Neighbors (KNN).
•	Time-Series Forecasting:
  •	SARIMA (Seasonal ARIMA): Strong in short-term seasonal variations.
  •	Prophet (Facebook): Effective in capturing long-term trends and uncertainty intervals.

3)	Evaluation Metrics:
•	MAE (Mean Absolute Error)
•	RMSE (Root Mean Squared Error)
•	MAPE (Mean Absolute Percentage Error)

## Results and Observations
•	Random Forest Regressor performed best among machine learning models.
•	SARIMA delivered high accuracy for short-term seasonal crime forecasting.
•	Prophet was effective for long-term trend forecasting and uncertainty estimation.
•	State wise NCRB anomalies (post-2018) made state-level forecasting unreliable; city-level and Kaggle datasets were more robust.

## Tech Stack
•	Languages: Python (Pandas, NumPy, Matplotlib, Seaborn)
•	ML/Forecasting Libraries: Scikit-learn, Prophet, Pmdarima
•	Data Sources: NCRB, Census, Kaggle.

## Future Scope and modifications
•	Improve anomaly detection for inconsistent reporting in NCRB data.
•	Explore deep learning approaches (LSTMs, Transformers) for multi-step forecasting.
•	Build an interactive dashboard for real-time crime trend monitoring.
