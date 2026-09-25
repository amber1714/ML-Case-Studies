# El Niño / La Niña Classification using Random Forest

## Objective

Use machine learning to classify ENSO conditions into:

- El Niño
- La Niña
- Neutral

The model uses historical Oceanic Niño Index-related features to predict the ENSO class.

## Dataset

The project uses an NOAA-derived ONI dataset containing seasonal ENSO information.

Main columns include:

- `Year`
- `Season`
- `ONI`
- `Season_Number`
- `ENSO_Class`
- `ONI_Lag1`
- `ONI_Lag2`
- `ONI_Lag3`
- `ONI_Rolling3_Previous`

## ENSO Classes

The dataset contains three classes:

- Neutral: 412 samples
- La Niña: 254 samples
- El Niño: 253 samples

## Features Used

The Random Forest model uses:

- `Season_Number`
- `ONI_Lag1`
- `ONI_Lag2`
- `ONI_Lag3`
- `ON
