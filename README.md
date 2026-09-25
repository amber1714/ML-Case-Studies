# El Niño / La Niña ML Analysis

Uses historical NOAA ONI data to classify ENSO conditions.

## Dataset
`data/ENSO_NOAA_ONI_1950_2026.csv`

## Key points
- El Niño / Neutral / La Niña classes
- Lagged ONI features
- Time-aware train/test split
- Random Forest classifier
- Accuracy, precision, recall, F1-score
- Confusion matrix
- Feature importance

## Important
The current ONI value is intentionally excluded from the ML input features because the target class was created from that value.
