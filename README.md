# Python-insurance-price-prediction

## 1. Introduction

### Background
In this project, we aim to predict individual medical costs billed by health insurance (charges) based on various demographic and health-related factors. The goal is to create a machine learning model that accurately predicts insurance charges, which can be valuable for insurance companies in pricing their policies effectively.

## Model comparison report
To compare the models - Linear Regression, Lasso Regression, XGB Regressor, Gradient Boosting Regressor, and their tuned versions, here is a summary of their performance metrics:

| Model                      | R-Squared (Test Score) | Mean Absolute Error | Mean Square Error | Root Mean Square Error |
|----------------------------|-------------------------|---------------------|-------------------|-------------------------|
| Linear Regression          | 0.446                   | 3368.09             | 29446640.95       | 5426.48                 |
| Lasso Regression           | 0.446                   | 3361.50             | 29465270.08       | 5428.19                 |
| XGB Regressor              | 0.603                   | 2502.65             | 21090395.26       | 4592.43                 |
| Gradient Boosting Regressor | 0.597                   | 2462.10             | 21412288.87       | 4627.34                 |
| XGB Regressor (Tuned)      | 0.514                   | 2592.98             | 25799972.73       | 5079.37                 |
| Gradient Boosting (Tuned)  | 0.527                   | 2393.54             | 24128917.63       | 4912.76                 |

From the R-squared values and error metrics, the Gradient Boosting Regressor (untuned) has a slightly higher R-squared value (0.603) and comparatively lower error metrics among the basic models. However, after tuning, the Gradient Boosting Regressor has improved slightly, with an R-squared value of 0.527 and lower errors compared to the untuned model.

Therefore, based on the provided data and analysis, the Gradient Boosting Regressor (tuned version) appears to be the best model for this prediction task, as it has a good balance between the R-squared value and lower errors.

### Overall Conclusion:

- **Best Performing Model:** The Gradient Boosting Regressor model after hyperparameter tuning yields the highest test score of 0.5279, indicating better predictive performance compared to other models.
- **Comparison:** Both XGBoost and Gradient Boosting models outperform Linear and Lasso regressions significantly, with Gradient Boosting showing a slightly better performance after tuning.

Based on these observations, the Gradient Boosting model, especially after hyperparameter tuning, stands out as the most effective model for the given dataset in predicting the target variable.

---