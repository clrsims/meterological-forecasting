## Rainfall-Next-Day Prediction | Kaggle Competition |  Python (scikit-learn, pandas, XGBoost).

Built an end‑to‑end ML pipeline (EDA → feature engineering → model training/validation → automated CSV submission) that boosted ROC‑AUC from 0.71 (logistic baseline) to 0.89 with XGBoost, ranking in the top 20 % of 2300 Kaggle teams.
- Engineered 20+ meteorological lag & interaction features (humidity/pressure trends, cloud–sunshine ratios, dew‑point flags) that increased model lift by 19 pp over raw inputs.
- Performed statistical EDA—heat‑maps, wind‑rose plots, joint‑density charts—to uncover key drivers (humidity, cloud cover, low pressure) and guide feature design.
- Applied ensemble methods (Random Forest, Gradient Boosting) and SHAP explainability to quantify feature importance, enabling domain experts to validate physical plausibility.

## Dataset

The used is from the **[Binary Prediction with a Rainfall Dataset](https://www.kaggle.com/competitions/playground-series-s5e3/data)** competition on Kaggle. It includes:
- 'train.csv' - the training dataset; rainfall is the binary target
- 'test.csv' - the test dataset; your objective is to predict the probability of rainfall for each row

## Installation

1. **Clone the repo**
 
    ```bash
    git clone https://github.com/clrsims/meterological-forecasting.git
    cd meterological-forecasting

2. **Install dependencies**
     ```bash
     pip install -r requirements.txt

3. **Prepare the dataset**
     ```bash
    rainfall-next-day-prediction/
    ├── data/
    │   ├── train.csv
    │   ├── test.csv
    ├── rainfall_pipeline.py
    ├── requirements.txt
    └── README.md

4. **Run the notebook**
     ```bash
     jupyter notebook
