## ⚡ AES Indiana Grid Load Forecasting Prototype

This repository presents a reproducible **short-term electricity load forecasting** workflow built to mirror the operational challenges faced by **AES Indiana** and other utilities. Using open MISO regional load data as a public proxy for AES’s grid demand, the notebook demonstrates an end-to-end process—data cleaning, feature engineering, baseline ARIMA modeling, and visual forecasting—implemented entirely in Python.

The goal is to provide a transparent, extendable foundation for future utility analytics work, enabling integration with internal AES data sources (SCADA, AMI, weather feeds) and more advanced forecasting techniques such as SARIMA, Prophet, or gradient-boosted models. All results are reproducible in a single Jupyter environment and export ready for dashboards or Power BI integration.

Key Deliverables in This Repo
•	Goal: Predict short-term utility grid load (daily/weekly) using open or synthetic data.
•	Core Models: ARIMA → SARIMA → RandomForestRegressor (optional).
•	Visualization: Matplotlib / Plotly (interactive dashboard).

