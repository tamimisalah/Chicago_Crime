
# 📊 Chicago Crime Analysis & Forecasting

This project performs an in-depth analysis and time series forecasting of crime data in the city of Chicago using Python. It includes crime trend insights, seasonal decomposition, rush hour comparisons, holiday effects, and SARIMA forecasting for selected crime types.

---

## 📁 Dataset

- Source: [Chicago Data Portal – Crimes 2001 to Present](https://data.cityofchicago.org)
- Data Format: One row per reported crime
- Includes: Crime type, datetime, location, arrest status, police district, etc.

---

## 📌 Part 1 – Exploratory Data Analysis (EDA)

This section answers key stakeholder questions such as:

### Topics Covered:
- 🔹 **District Crime Volume (2022)** – Which districts are most and least affected
- 🔹 **Yearly Crime Trends** – Whether overall crime is increasing or decreasing
- 🔹 **AM vs PM Rush Hour Analysis** – Time-of-day trends and common crime types
- 🔹 **Monthly Seasonality** – Which months are worst, and anomalies by crime type
- 🔹 **Holiday Impact** – Top holidays with the highest crime counts
- 🔹 **Cycle Detection** – Seasonal decomposition of total and per-crime data

---

## 📌 Part 2 – Forecasting

We forecast the next 6 months of crime counts using SARIMA and auto_arima.

### Crimes Forecasted:
- THEFT
- BATTERY

### Steps:
1. Monthly aggregation with `.resample('MS')`
2. Seasonal decomposition with `statsmodels`
3. Manual SARIMA modeling
4. Model diagnostics: ACF, PACF, RMSE
5. Auto tuning with `pmdarima.auto_arima`
6. Future forecasts + interpretation of change

---

## 📈 Visualizations

- Year-over-year crime trends
- AM vs PM crime type comparisons
- Heatmaps of district-level activity
- Monthly and seasonal cycle plots
- Forecasted trends vs test sets

---

## 📊 Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- pmdarima
- holidays

---

## 🧾 Final Outputs

- ✅ Top crime patterns over years, months, rush hours, holidays
- ✅ Forecast for 6 months ahead for THEFT & BATTERY
- ✅ Net and percent change interpretation
- ✅ Data-driven recommendation for law enforcement resource planning

---

## 📂 How to Use

1. Upload the dataset `.zip` to your Google Drive
2. Open the notebook in [Google Colab](https://colab.research.google.com)
3. Mount Drive and unzip the data
4. Run all cells step-by-step

---

## 📌 Author

Salah Aburajab

Prepared by a data scientist using Python, pandas, statsmodels, and real-world datasets for forecasting and EDA.

---

