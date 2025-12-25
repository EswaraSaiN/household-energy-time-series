# Household Power Consumption Forecasting

## 📌 Problem Statement
This project focuses on forecasting **hourly household electricity consumption** using historical power usage data.  
The goal is to predict the next **7 days of energy demand** based on nearly **4 years of past observations (2006–2010)**, enabling a better understanding of consumption patterns and preparing the data for time-series modeling.
> Note: This project currently focuses on univariate forecasting. In later
stages, additional household features will be incorporated as exogenous
variables to improve forecast accuracy.

---

## 📊 Dataset
- **Source**: UCI Machine Learning Repository  
- **Description**: Minute-level electricity consumption recorded from a single household
- **Size**: ~2.07 million observations
- **Time Range**: December 2006 – November 2010
- **Target Variable**: `Global_active_power` (kilowatts)
- **Preprocessing**:
  - Parsed and validated datetime index
  - Aggregated minute-level data to **hourly averages**
  - Handled missing values after resampling

---

## 🔧 Current Progress
- ✅ Data ingestion and cleaning
- ✅ Datetime parsing and validation
- ✅ Hourly resampling
- ✅ Exploratory Data Analysis (EDA)
- ✅ Visualizations:
  - Full time-series overview
  - January 2007 close-up
  - Hour-of-day consumption pattern
- 🔄 Next steps:
  - Final missing-value treatment
  - Stationarity testing
  - Time-series decomposition

---

## 🔍 Key Findings
- Strong **daily and weekly seasonality** driven by household activity
- Consistent **morning (7–9 AM)** and **evening (6–9 PM)** consumption peaks
- Lower energy usage during nighttime hours
- No strong long-term upward trend; consumption varies primarily with seasonal patterns

