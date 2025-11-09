# Sleep Quality Prediction Using XGBoost

## Project Overview
This project delivers a highly accurate sleep quality prediction model leveraging XGBoost, trained on a comprehensive health and lifestyle dataset. It uses advanced preprocessing, class balancing, and hyperparameter optimization to ensure reliable classification across four sleep quality levels: `Poor`, `Fair`, `Good`, and `Excellent`.

---

## Key Features
- Robust data preprocessing: encoding categorical features, handling missing values.
- Class imbalance handling using SMOTE.
- Hyperparameter tuning with GridSearchCV.
- Comprehensive evaluation: accuracy, precision, recall, F1-score, confusion matrix.
- Model persistence using Joblib.
- Visualization of confusion matrix.
- Extendable for web integration or further ML pipelines.

---

## Dataset Overview
Includes features like Age, Gender, Coffee Intake, BMI, Stress Level, Occupation, Smoking, Alcohol Consumption, and others affecting sleep quality.

---

## Model Accuracy

| Metric   | Score      |
|----------|------------|
| Accuracy | **99.67%** |

The model demonstrates excellent accuracy on test data, reflecting its strong generalization and prediction capabilities.

---

## Detailed Metrics on Test Set

| Metric    | Score   |
|-----------|---------|
| Precision | 99.67%  |
| Recall    | 99.67%  |
| F1 Score  | 99.67%  |

---

## Classification Report Snapshot

| Class        | Precision | Recall | F1-Score | Support |
|--------------|-----------|--------|----------|---------|
| Poor (0)     | 1.00      | 1.00   | 1.00     | 1128    |
| Fair (1)     | 1.00      | 1.00   | 1.00     | 1127    |
| Good (2)     | 1.00      | 0.99   | 0.99     | 1128    |
| Excellent (3)| 0.99      | 1.00   | 0.99     | 1127    |

---

## Best Hyperparameters
```json
{
  "learning_rate": 0.2,
  "max_depth": 10,
  "n_estimators": 150
}
