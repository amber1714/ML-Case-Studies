# Machine Learning Case Studies

Four Google Colab-ready machine-learning case studies.

## Projects

### 1. KNN Regression
California Housing price prediction using K-Nearest Neighbors with automated K comparison.

### 2. Linear, Ridge and Lasso Regression
Comparison of standard linear regression with L1/L2 regularization.

### 3. Intelligent Cleaning Robot
Q-Learning simulation showing reinforcement learning through rewards and penalties.

### 4. El Niño / La Niña ML Analysis
Random Forest classification using historical NOAA Oceanic Niño Index data and lagged features.

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
│   ├── Cleaning_Robot_Q_Learning.ipynb
│   └── README.md
├── 04_El_Nino_La_Nina/
│   ├── ENSO_ML_Analysis.ipynb
│   ├── README.md
│   └── data/
│       └── ENSO_NOAA_ONI_1950_2026.csv
├── requirements.txt
├── .gitignore
└── README.md
```

## Tools

Python, Google Colab, NumPy, Pandas, Matplotlib and Scikit-learn.

## How to Use

Open any `.ipynb` notebook in Google Colab and run the cells from top to bottom. The ENSO notebook requires the CSV stored in its `data` folder.
