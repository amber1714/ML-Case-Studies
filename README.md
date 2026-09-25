# Machine Learning Case Studies

A collection of four machine learning case studies implemented in Python and Google Colab. The repository covers supervised learning, regularization, reinforcement learning, and climate-data classification.

## Projects

### 1. KNN Regression — California Housing
- Algorithm: K-Nearest Neighbors Regression
- Dataset: California Housing
- Preprocessing: train/test split and feature standardization
- Model selection: K values from 1 to 30
- Best K: 13
- MAE: 0.4373
- RMSE: 0.6452
- R²: 0.6823

### 2. Linear, Ridge and Lasso Regression
- Dataset: California Housing
- Models: Linear Regression, Ridge Regression, Lasso Regression
- Metrics: MAE, MSE, RMSE and R²
- Best tested Ridge alpha: 100
- Best tested Lasso alpha: 0.01
- Best tested R²: approximately 0.5816 with Lasso
- Includes coefficient comparison and regularization analysis

### 3. Cleaning Robot using Q-Learning
- Technique: Reinforcement Learning
- Environment: 5 × 5 grid
- Actions: Up, Down, Left, Right and Clean
- Learning algorithm: Q-Learning
- Reward design encourages cleaning dirty cells while penalizing unnecessary movement and actions
- Includes a reward-learning curve to visualize training progress

### 4. El Niño / La Niña Classification
- Algorithm: Random Forest Classifier
- Data: NOAA Oceanic Niño Index-derived dataset
- Classes: El Niño, La Niña and Neutral
- Features: season number and lagged ONI indicators
- Test accuracy: approximately 85.6%
- El Niño F1-score: 0.92
- Most important feature: ONI_Lag1, with importance approximately 44.6%
- Includes confusion matrix and feature-importance analysis

## Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- scikit-learn
- Git and GitHub

## Repository Structure

```text
ML-Case-Studies/
├── 01_KNN/
│   ├── KNN_Regression.ipynb
│   └── README.md
├── 02_Regression/
│   ├── Linear_Ridge_Lasso.ipynb
│   └── README.md
├── 03_Cleaning_Robot/
│   └── Cleaning_Robot_Q_Learning.ipynb
├── 04_El_Nino_La_Nina/
│   ├── ENSO_ML_Analysis.ipynb
│   └── data/
├── README.md
└── requirements.txt
