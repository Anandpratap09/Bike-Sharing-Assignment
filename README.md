# Bike Sharing Demand: Multiple Linear Regression

Explains which factors drive daily shared-bike demand in the US market, so a bike-sharing provider can plan for demand after the COVID-19 lockdown.

## Questions answered

- Which variables significantly predict bike demand?
- How well do those variables explain demand?

## Approach

1. Visualize numeric and categorical variables against demand (`cnt`)
2. Prepare data: dummy variables, train/test split, scaling
3. Build the model by feature elimination, checking VIF and p-values (final model `lr_6`)
4. Residual analysis: normality of errors, multicollinearity, linearity, homoscedasticity, independence
5. Predict on the test set and compare train and test performance

## Results

| Metric | Train | Test |
| --- | --- | --- |
| R² | 0.833 | 0.804 |
| Adjusted R² | 0.829 | 0.794 |

The Durbin-Watson statistic is 2.085, so there is no sign of autocorrelation in the residuals. Season and month were among the strongest categorical drivers in the exploratory analysis.

## Files

| File | Purpose |
| --- | --- |
| `Bike sharing Assigment_anand.ipynb` | Full analysis |
| `Linear_Regression_Subjective_Questions(Anand).pdf` | Written answers |

## Stack

Python, pandas, scikit-learn, statsmodels, matplotlib, seaborn
