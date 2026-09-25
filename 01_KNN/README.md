# KNN Regression — California Housing

## Objective

Use K-Nearest Neighbors Regression to predict median house values from the California Housing dataset and determine an effective value of K.

## Dataset

- Dataset: California Housing
- Target variable: `MedHouseVal`
- Features include median income, house age, average rooms, population, occupancy, latitude, and longitude.

## Preprocessing

- Split the dataset into training and testing sets.
- Standardized the features using `StandardScaler`.
- Feature scaling is important for KNN because the algorithm relies on distance calculations.

## Algorithm

KNN Regression predicts a value by finding the K nearest training samples and averaging their target values.

Different values of K from 1 to 30 were tested.

## Best K

The selected value was:

- Best K: 13

This value produced the lowest RMSE among the tested K values.

## Results

- MAE: 0.4373
- MSE: 0.4163
- RMSE: 0.6452
- R²: 0.6823

The R² score indicates that the model explains approximately 68.2% of the variation in median house values.

## Visualization

The notebook includes:

- RMSE comparison for different K values
- Actual vs Predicted house-value graph

## Inference

A very small K can make the model sensitive to noise, while a very large K can over-smooth predictions. Testing multiple K values helped identify K = 13 as a suitable value for this experiment.

## Tools Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- scikit-learn

## Conclusion

KNN Regression achieved reasonable predictive performance on the California Housing dataset. Feature standardization and K-value selection were important for improving the model's performance.
