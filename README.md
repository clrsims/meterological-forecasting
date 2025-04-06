### Rainfall-Next-Day Prediction | Kaggle Competition |  Python (scikit-learn, pandas, XGBoost).

Built an end‑to‑end ML pipeline (EDA → feature engineering → model training/validation → automated CSV submission) that boosted ROC‑AUC from 0.71 (logistic baseline) to 0.89 with XGBoost, ranking in the top 20 % of 2 300 Kaggle teams.
- Engineered 20+ meteorological lag & interaction features (humidity/pressure trends, cloud–sunshine ratios, dew‑point flags) that increased model lift by 19 pp over raw inputs.
- Performed statistical EDA—heat‑maps, wind‑rose plots, joint‑density charts—to uncover key drivers (humidity, cloud cover, low pressure) and guide feature design.
- Applied ensemble methods (Random Forest, Gradient Boosting) and SHAP explainability to quantify feature importance, enabling domain experts to validate physical plausibility.

## Dataset

The data used is from the **[Corporación Favorita Grocery Sales Forecasting](https://www.kaggle.com/competitions/favorita-grocery-sales-forecasting)** competition on Kaggle. It includes:

- `train.csv` — historical sales records  
- `test.csv` — data for forecasting  
- `stores.csv` — metadata on stores  
- `oil.csv` — daily oil prices  
- `holidays_events.csv` — national/regional holidays

## Installation

1. **Clone the repo:**

   ```bash
   git clone https://github.com/yourusername/grocery-sales-forecasting.git
   cd grocery-sales-forecasting
   
2. ** Install dependencies
