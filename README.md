Bangladesh Dengue Forecasting (Time-Series Regression + SARIMA)

This repository contains code for a dengue forecasting analysis for Bangladesh using:
- log(1+cases) transformation
- autoregressive lag features
- seasonal sin/cos encoding
- lagged climate covariates (NASA POWER)
- rolling-origin (walk-forward) validation
- SARIMA benchmark with prediction intervals
- statistical diagnostics (ADF, Ljung–Box, Breusch–Pagan)

Data sources
- Dengue surveillance data: OpenDengue (https://opendengue.org)
- Climate data: NASA POWER API (https://power.larc.nasa.gov)

How to run
1) Create a virtual environment (optional)
2) Install dependencies:
   pip install -r requirements.txt
3) Place dengue dataset CSV in the project root named:
   dengue dataset.csv
4) Run:
   python run_analysis.py

Outputs
Figures are displayed during execution and may be saved to outputs/figures if desired.
