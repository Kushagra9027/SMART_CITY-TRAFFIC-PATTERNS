# Week 03 Progress Report

## Project

Smart City Traffic Forecasting

## Duration

Week 03

---

## Objectives

The objective of Week 03 was to develop and evaluate baseline machine learning models for traffic volume prediction using the prepared traffic dataset.

---

## Activities Completed

### 1. Data Preparation

* Prepared features for machine learning model development.
* Selected relevant temporal and spatial features:

  * Junction
  * Year
  * Month
  * Day
  * Hour
  * Weekday
* Defined Vehicle Count as the target variable.
* Performed train-test splitting for model evaluation.

---

### 2. Linear Regression Model

Implemented Linear Regression as the baseline forecasting model.

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 9.75  |
| RMSE     | 13.00 |
| R² Score | 0.585 |

#### Observations

* Successfully captured general traffic patterns.
* Explained approximately 58.5% of traffic variation.
* Served as a baseline for comparison with more advanced models.

---

### 3. Random Forest Regressor

Implemented Random Forest Regressor to model complex non-linear traffic relationships.

#### Performance

| Metric   | Value |
| -------- | ----- |
| MAE      | 2.40  |
| RMSE     | 3.59  |
| R² Score | 0.968 |

#### Observations

* Significantly outperformed Linear Regression.
* Achieved very low prediction error.
* Successfully captured complex traffic patterns across different junctions and time periods.

---

### 4. Model Comparison

| Model                   | MAE  | RMSE  | R² Score |
| ----------------------- | ---- | ----- | -------- |
| Linear Regression       | 9.75 | 13.00 | 0.585    |
| Random Forest Regressor | 2.40 | 3.59  | 0.968    |

#### Result

Random Forest Regressor achieved the best performance and was selected as the current best model.

---

### 5. Feature Importance Analysis

Performed feature importance analysis using the Random Forest model.

#### Feature Importance Ranking

| Feature  | Importance |
| -------- | ---------- |
| Junction | 0.517      |
| Year     | 0.166      |
| Hour     | 0.145      |
| Weekday  | 0.071      |
| Month    | 0.068      |
| Day      | 0.033      |

#### Key Findings

* Junction was identified as the most influential predictor.
* Temporal features such as Hour and Weekday also contributed significantly.
* Traffic volume is strongly influenced by both location and time.

---

### 6. Prediction Visualization

Generated Actual vs Predicted Traffic Volume visualization.

#### Observations

* Most predictions closely followed the ideal prediction line.
* Strong agreement observed between actual and predicted traffic counts.
* Limited prediction error observed for higher traffic volumes.

---

## Key Learnings

During Week 03, I learned:

* Regression model development.
* Linear Regression implementation.
* Random Forest Regression implementation.
* Model evaluation using MAE, RMSE, and R².
* Feature importance analysis.
* Traffic forecasting workflow.
* Model comparison techniques.

---

## Challenges Faced

* Selecting meaningful temporal features.
* Understanding feature importance interpretation.
* Evaluating forecasting model performance.

---

## Planned Activities for Week 04

* Hyperparameter tuning.
* Model optimization.
* Feature engineering improvements.
* Additional forecasting model experimentation.
* Performance enhancement.
* Final report preparation.

---

## Status

Week 03 successfully completed.

Baseline forecasting models have been developed and evaluated. Random Forest Regressor currently provides excellent forecasting performance with an R² score of 0.968 and is selected as the best-performing model for further optimization.
