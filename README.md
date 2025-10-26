# ☀️ Solar Index Prediction for Mumbai

An end-to-end machine learning pipeline for predicting solar irradiance in Mumbai using time series analysis and feature engineering. This project fetches real-time data from NASA POWER API and prepares it for solar energy forecasting models.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## 🌟 Overview

This project implements a complete workflow for solar energy prediction in Mumbai regions, specifically focusing on Ghatkopar. The system processes historical solar irradiance data to create predictive models that can help in solar energy planning and optimization.

**Key Objectives:**
- Fetch and process real-time solar data from NASA POWER API
- Perform comprehensive exploratory data analysis
- Engineer temporal and statistical features for machine learning
- Create a foundation for accurate solar energy forecasting

## 🚀 Features

- **Automated Data Pipeline**: Fetches 3 years of solar irradiance data (2022-2025)
- **Advanced Feature Engineering**: 41+ temporal and statistical features
- **Comprehensive EDA**: 10+ visualization plots for data insights
- **Data Preprocessing**: Handles missing values and data quality checks
- **Time Series Analysis**: Lag features, rolling statistics, and seasonal decomposition
- **Machine Learning Ready**: Processed dataset for forecasting models

## 📊 Dataset

**Source**: NASA POWER API (Prediction Of Worldwide Energy Resources)

**Parameters:**
- **Measurement**: All-Sky Surface Shortwave Downward Irradiance
- **Unit**: kWh/m²/day
- **Location**: Ghatkopar, Mumbai (19.086°N, 72.9081°E)
- **Date Range**: 2022-10-27 to 2025-10-26
- **Records**: 1,096 days (1,060 after preprocessing)

**Statistical Summary:**
- Mean: 4.97 kWh/m²/day
- Median: 5.01 kWh/m²/day
- Standard Deviation: 1.50 kWh/m²/day
- Range: 0.31 - 7.75 kWh/m²/day

## 🛠️ Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook

### Dependencies

pip install pandas numpy matplotlib seaborn requests scikit-learn statsmodels

## 📖 Usage
The project follows a **sequential workflow**:

1. **Data Acquisition:** Fetch solar data from NASA POWER API  
2. **Preprocessing:** Clean and validate the dataset  
3. **Feature Engineering:** Create temporal and statistical features  
4. **EDA:** Generate insights through visualizations  
5. **Model Preparation:** Prepare data for machine learning  

> 💡 Execute the cells in `solar_index_predictions.ipynb` **in order** to reproduce the entire pipeline.

---

## 🔬 Methodology

### 🧩 Feature Engineering
- **Temporal Features:** Year, Month, Day, Week, Quarter  
- **Seasonal Classification:** Automatic season labeling  
- **Lag Features:** 1, 2, 3, 7, 14, and 30 days  
- **Rolling Statistics:** 3, 7, 14, 30-day windows (mean, std)  
- **Exponential Weighted Moving Averages (EWMA)**  
- **Weather Interaction Features**

### ⚙️ Data Processing Pipeline
1. Fetch data from **NASA POWER API**  
2. Perform **quality checks** and handle missing values  
3. Generate **temporal features**  
4. Create **statistical and lag features**  
5. Validate processed data and **export clean dataset**

---

## 📈 Results

The project successfully:
- ✅ Fetched **1,096 days** of solar irradiance data  
- ✅ Processed and cleaned dataset (**1,060 valid records**)  
- ✅ Engineered **41 predictive features**  
- ✅ Created **comprehensive EDA visualizations**  
- ✅ Established a **foundation for machine learning models**

### 📊 Sample Visualizations
- Time series overview of solar index  
- Seasonal patterns and trends  
- Distribution analysis  
- Correlation studies  

---

## 🔮 Future Work
- Implement ML models: **ARIMA**, **Prophet**, **LSTM**, **XGBoost**  
- Hyperparameter tuning and model optimization  
- Develop a **forecasting web application**  
- Extend to **multiple locations across India**  
- Build a **real-time prediction API**  
- Integrate with **solar energy management systems**

---

## 🤝 Contributing
Contributions are welcome! 🎉  
Please feel free to submit a **Pull Request**. For major changes, open an **issue** first to discuss what you’d like to modify.

1. **Fork** the project  
2. Create your feature branch  
   ```bash
   git checkout -b feature/AmazingFeature
