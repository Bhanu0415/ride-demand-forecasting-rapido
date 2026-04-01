# 🚀 Ride Demand Forecasting & Dynamic Surge Pricing

Built for Rapido Data Science Internship application.

## 📌 Problem Statement
Predict hourly ride demand across city zones and dynamically
calculate surge pricing multipliers based on demand-supply ratio.

## 📊 Dataset
- 500,000 simulated ride records based on real ride-hailing patterns
- Features: hour, day, zone, weather, vehicle type, holidays

## 🔍 Key Findings from EDA
- Evening rush (5PM–9PM) shows highest demand — 20+ extra rides/hour
- Rainfall increases demand by ~12 rides/hour
- Airport and Downtown zones have consistently highest demand
- Weekend demand is 8 rides/hour higher than weekdays

## 🤖 Model Performance
| Metric | Score |
|--------|-------|
| Algorithm | XGBoost Regressor |
| MAE | 2.37 rides |
| RMSE | 2.97 rides |
| R² Score | 0.9484 (94.84% accuracy) |

## 💰 Surge Pricing Engine
| Demand/Driver Ratio | Multiplier | Level |
|---------------------|------------|-------|
| < 0.8 | 1.0x | Normal |
| 0.8 – 1.2 | 1.5x | Moderate |
| 1.2 – 1.8 | 2.0x | High |
| > 1.8 | 3.0x | Very High |

## 🛠️ Tech Stack
Python · XGBoost · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn

## 📁 Project Structure
- `demand_forecasting.ipynb` — Full notebook (EDA + Feature Engineering + Model)
- `xgb_demand_model.pkl` — Saved trained model
- `eda_analysis.png` — EDA visualizations
- `model_results.png` — Model performance charts
- `project_report.json` — Detailed summary report

## 🚀 How to Run
1. Open `demand_forecasting.ipynb` in Google Colab
2. Run all cells in order
3. Model trains in ~30 seconds
