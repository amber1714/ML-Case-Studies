# Linear, Ridge and Lasso Regression — California Housing

## Objective

Compare Linear Regression, Ridge Regression, and Lasso Regression on the California Housing dataset and study the effect of regularization.

## Dataset

- Dataset: California Housing
- Target variable: `MedHouseVal`
- Features include median income, house age, average rooms, population, occupancy, latitude, and longitude.

## Preprocessing

- Split the dataset into training and testing sets.
- Standardized the features using `StandardScaler`.

## Models Used

### Linear Regression
Standard regression without regularization.

### Ridge Regression
Uses L2 regularization to shrink model coefficients and reduce overfitting.

### Lasso Regression
Uses L1 regularization and can reduce some coefficients to zero, which can also help with feature selection.

## Evaluation Metrics

The models were evaluated using:

- MAE
- MSE
- RMSE
- R² Score

## Results

| Model | MAE | MSE | RMSE | R² |
|---|---:|---:|---:|---:|
| Linear Regression | 0.5332 | 0.5559 | 0.7456 | 0.5758 |
| Ridge Regression | 0.5332 | 0.5559 | 0.7456 | 0.5758 |
| Lasso Regression | 0.5353 | 0.5483 | 0.7404 | 0.5816 |

Among the tested configurations, Lasso Regression produced the highest R² score.

## Alpha Analysis

Different alpha values were tested for Ridge and Lasso.

### Ridge
Best tested alpha:

- Alpha = 100
- R² ≈ 0.5778

### Lasso
Best tested alpha:

- Alpha = 0.01
- R² ≈ 0.5816

## Coefficient Analysis

Ridge reduced the magnitude of coefficients but retained all features.

Lasso reduced some coefficients more aggressively and set the `Population` coefficient to zero.

This demonstrates how L1 regularization can perform a form of feature selection.

## Visualization

The notebook includes:

- R² model comparison
- Alpha comparison
- Ridge and Lasso coefficient analysis

## Tools Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- scikit-learn

## Conclusion

Regularization slightly affected the regression performance on the California Housing dataset. Lasso Regression with alpha = 0.01 achieved the highest R² among the tested settings and also demonstrated coefficient sparsity.
