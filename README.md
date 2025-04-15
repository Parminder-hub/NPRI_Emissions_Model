# NPRI_Emissions_Model
# 🌍 NPRI Emissions Model

## 📌 Objective
Forecast pollutant release levels from fossil fuel electricity generation using time-series data from Canada’s National Pollutant Release Inventory (NPRI).  
This model estimates environmental impact trends and simulates emission reductions if coal plants are phased out by 2030.

---

## 🗂️ Dataset
- **Source**: [NPRI (Canada)](https://pollution-waste.canada.ca/national-release-inventory/)
- **Years Covered**: 2000–2022
- **Filtered by NAICS Code**: 221112 – Fossil Fuel Electric Power Generation
- **File Used**: `release_dataset.csv`

---

## ⚙️ Tech Stack
- **Language**: Python
- **Tools**: Jupyter Notebooks
- **Libraries**: pandas, NumPy, scikit-learn, matplotlib, seaborn
- **Modeling Techniques**: Linear Regression, Decision Tree, Random Forest
- **Data Prep**: Feature engineering, scaling, and time-based train-test split

---

## 🔬 Key Features
- Time-series cleaning (interpolation, outlier handling, missing value imputation)
- Date-based and rolling window feature engineering
- Built and compared multiple regression models
- Evaluated using R², MAE, RMSE, and Accuracy
- Visual analysis of predictions and trends

---

## 📊 Model Performance

| Model              | MAE     | RMSE    | R²     | Accuracy |
|-------------------|---------|---------|--------|----------|
| Linear Regression | 2291.28 | 2748.41 | 0.476  | 95.76%   |
| Decision Tree     | 3314.93 | 4143.36 | -0.190 | 93.86%   |
| Random Forest     | 3192.23 | 3994.64 | -0.106 | 94.09%   |

✅ **Linear Regression** outperformed others with the highest R² and lowest error metrics.

---

## 📈 Visualizations
- Year-wise emission trend line charts
- Correlation heatmaps
- Predicted vs. actual emissions
- Feature importance (Random Forest)

> 📸 Example:
> ![Emissions Forecast](images/emissions_forecast.png)

---

## 📁 How to Run This Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/NPRI_Emissions_Model.git
