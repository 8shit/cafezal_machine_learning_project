# ☕ Cafezal Sales Forecasting and Peak Prediction Project

This project uses machine learning to predict daily sales, identify peak days and hours, and evaluate weather impact across multiple Cafezal branches in Milan. Built as part of an internal data science initiative, this model aims to support operational planning, marketing optimization, and future digital product development.

---

## 📌 Objectives

- Forecast daily and hourly sales for all Cafezal branches.
- Identify peak days and hours with high confidence.
- Evaluate branch-to-branch performance and correlations.
- Integrate external data (weather) to enhance forecasting.
- Deliver actionable business insights for internal decision-making.

---

---

## 🔧 Models Used

- **Random Forest Regressor**  
  For predicting daily and hourly total sales across branches.

- **Random Forest Classifier**  
  For peak day and peak hour classification (80th percentile threshold).

- **Cross-Validation Metrics:**  
  - R² CV Score (Daily Forecasting): ~0.85  
  - F1 CV Score (Peak Classification): ~0.78 (daily), ~0.36 (hourly)

---

## 📈 Key Results

| Branch               | Test R² | Test RMSE (€) |
|----------------------|---------|----------------|
| CAFEZAL_PREMUDA       | 0.86    | 284.82         |
| CAFEZAL_SOLFERINO     | 0.79    | 211.46         |
| CAFEZAL_S_GREGORIO    | 0.59    | 164.11         |
| CAFEZAL_CSO_MAGENTA   | 0.48    | 121.49         |

- 🌦️ Weather slightly improved performance (+0.3–0.5% R²)
- 📊 April 2025 forecasts were generated with realistic sales curves per branch
- 🟢 Peak days and hours identified with probability scores

---

## 📅 April Forecasts

Each branch has:
- **CSV** with forecasted daily sales (`April_Forecasts/`)
- **Graph** showing trends (`April_Forecast_Plots/`)

---

## 🌍 External Data

- **Weather data** scraped from Milan between April 2024 and April 2025
- Integrated features:
  - Temperature (avg)
  - Humidity
  - Precipitation
  - Wind speed
  - Weather conditions (encoded)

---

## 📊 Future Improvements

- Integrate marketing campaign data post–app launch
- Improve hourly model with true intra-day data granularity
- Build API layer for real-time forecasting + alerting
- Incorporate calendar holidays & events

---

## 🧠 Contributors

- **Alexander Dagher** — Data Analyst & Machine Learning Intern  
  Cafezal Coffee | February 2025 – May 2025

---

## 📫 Contact

For questions, business use, or further development:  
**dagher3@stolaf.edu**
