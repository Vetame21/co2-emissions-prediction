# CO2 Emissions Prediction

Predicting a car's CO2 emissions (g/km) from its specs and fuel consumption, using linear regression.

## Data
`co2.csv`: 7,385 car models with brand, vehicle class, engine size, cylinders, transmission, fuel type and fuel consumption. It's the "CO2 Emission by Vehicles" dataset from Kaggle, based on data from the Government of Canada.

## What I did
- Checked for missing values (none) and dropped 1,103 duplicate rows, leaving 6,282
- Explored the data: distributions, CO2 by brand, vehicle class and transmission type
- Built a scikit-learn pipeline: one-hot encoding for the categorical columns, then linear regression
- Split the data 75/25 into train and test sets and evaluated on the test set

## Results (test set)
| Metric | Value |
|---|---|
| R² | 0.990 |
| MAE | 3.6 g/km |
| RMSE | 6.1 g/km |

## Run it
```
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook co2_emissions.ipynb
```
