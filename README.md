### Rainfall-Next-Day Prediction | Kaggle Competition |  Python (scikit-learn, pandas, XGBoost).

Built an end‑to‑end ML pipeline (EDA → feature engineering → model training/validation → automated CSV submission) that boosted ROC‑AUC from 0.71 (logistic baseline) to 0.89 with XGBoost, ranking in the top 20 % of 2 300 Kaggle teams.
- Engineered 20+ meteorological lag & interaction features (humidity/pressure trends, cloud–sunshine ratios, dew‑point flags) that increased model lift by 19 pp over raw inputs.
- Performed statistical EDA—heat‑maps, wind‑rose plots, joint‑density charts—to uncover key drivers (humidity, cloud cover, low pressure) and guide feature design.
- Applied ensemble methods (Random Forest, Gradient Boosting) and SHAP explainability to quantify feature importance, enabling domain experts to validate physical plausibility.

![image](https://github.com/user-attachments/assets/8dc1b820-9038-4646-a17a-0961c6e89e01)

![image](https://github.com/user-attachments/assets/681ee61c-0fe0-46ed-a012-37689d51bc20)

From my data analysis, I engineered new features to increase the accuracy of my model, with an emphasis on lag and composite features. On weather data, temporal features are especially important. From there, I split my data into a training and testing set, performed feature scaling to minimize the effect of scaling on feature importance.  

From here, I designed and trained a logistic regression, random forest, and XGBoost (Gradient Boosted Forest) model to get different baselines. For each, I graphed the relevant feature importance (how much each feature contributed to minimizing cost) and specifically analyzed my XGBoost model using SHAP. From there, I removed features with low importance to remove noise from my model.  

![image](https://github.com/user-attachments/assets/e407ae94-6edd-46f9-9de2-db5a9f6e25a0)

![image](https://github.com/user-attachments/assets/5f100e84-5d3f-4741-b842-164166b90f0e)

I calculated my final AUC score (area under the Receiver Operating Characteristic curve, and submitted my score, landing in the top 10% of all Kaggle submissions.

![image](https://github.com/user-attachments/assets/f59eac1b-fe84-48cb-b3fc-2d35004e655c)

Tech stack: Jupyter Notebooks, Python (pandas, seaborn, matplotlib, scikit-learn, and xgboost).  

Techniques used: exploratory data analysis, statistical modeling, feature engineering, time-series & lag feature creation, model training, data scaling & preprocessing, XGBoost, logisitic regression, data engineering, and SHAP.
