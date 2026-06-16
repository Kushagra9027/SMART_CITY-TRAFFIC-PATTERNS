# Week 04 Progress Report

## Project

Smart City Traffic Forecasting

## Duration

Week 04

---

## Objectives

The objective of Week 04 was to optimize forecasting models, evaluate advanced machine learning algorithms, compare model performance, and select the final model for traffic volume prediction.

---

## Activities Completed

### 1. Random Forest Optimization

The Random Forest model developed during Week 03 was further evaluated and validated as the primary forecasting model.

Key Parameters:

```python
RandomForestRegressor(
    n_estimators=200,
    random_state=42,
    n_jobs=-1
)
```

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 2.40  |
| RMSE     | 3.59  |
| R² Score | 0.968 |

#### Observations

* Achieved very high prediction accuracy.
* Successfully captured traffic patterns across different junctions.
* Demonstrated strong generalization performance.

---

### 2. XGBoost Regressor Implementation

An XGBoost Regressor was implemented to evaluate whether further performance improvements could be achieved.

```python
from xgboost import XGBRegressor
```

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 2.76  |
| RMSE     | 4.62  |
| R² Score | 0.948 |

#### Observations

* Produced strong forecasting performance.
* However, performance remained below Random Forest.
* Higher prediction error compared to the Random Forest model.

---

### 3. Model Comparison

| Model                   | MAE  | RMSE  | R² Score |
| ----------------------- | ---- | ----- | -------- |
| Linear Regression       | 9.75 | 13.00 | 0.585    |
| Random Forest Regressor | 2.40 | 3.59  | 0.968    |
| XGBoost Regressor       | 2.76 | 4.62  | 0.948    |

---

### 4. Final Model Selection

After comparing all evaluated models, Random Forest Regressor was selected as the final forecasting model.

#### Selected Model

**Random Forest Regressor**

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 2.40  |
| RMSE     | 3.59  |
| R² Score | 0.968 |

#### Reasons for Selection

* Lowest prediction error.
* Highest R² Score.
* Most stable forecasting performance.
* Successfully captured temporal and spatial traffic patterns.

---

## Key Findings

* Junction was identified as the most influential predictor of traffic volume.
* Hour and Year also contributed significantly to forecasting accuracy.
* Random Forest consistently outperformed alternative models.
* Traffic volume can be predicted with high accuracy using machine learning techniques.
* The forecasting model successfully explains approximately 96.8% of traffic variation.

---

## Challenges Faced

* Comparing multiple regression algorithms.
* Understanding model evaluation metrics.
* Interpreting forecasting performance differences.
* Selecting the most suitable final model.

---

## Learning Outcomes

During Week 04, I learned:

* Model optimization techniques.
* Ensemble learning methods.
* XGBoost implementation.
* Model comparison and selection.
* Forecasting model evaluation.
* Advanced traffic prediction techniques.

---

## Project Status

Week 04 successfully completed.

The final forecasting model has been selected and evaluated. Random Forest Regressor achieved the best overall performance and was selected as the final model for Smart City Traffic Forecasting.

The project is now ready for final documentation and report preparation.
