# Glass Identification Classification

## About
This dataset is taken from UCI Machine Learning repository.

This dataset is about classifying various types of glass by using features like: 
- RI: refractive index
- Na: Sodium
- Mg: Magnesium
- Al: Aluminum
- Si: Silicon
- K: Potassium
- Ca: Calcium
- Ba: Barium
- Fe: Iron 

Types of glass we have to classify:
- building_windows_float_processed
- building_windows_non_float_processed
- vehicle_windows_float_processed
- vehicle_windows_non_float_processed (none in this database)
- containers
- tableware
- headlamps

## What I have done
The data which I have taken is already clean data so there's nothing to clean.
So, I split data into 2 parts:
- X contains features like RI,Na,Mg,Al etc.
- y contains target which we have to classify.

Then I trained models using X and y.

1) Logistic Regression
- Trained data using *logistic regression* with hyperparameter max_iter=5000, solver=saga
- F1 score 0.47,0.50,0.00,0.00,0.00,0.90
- Accuracy: 0.52

2) K Nearest Neighbors
- Trained data using *K Nearest Neighbors* with hyperparameter n_neighbors=16
- F1 score 0.62,0.71,0.40,0.40,0.00,0.82
- Accuracy: 0.67

3) Decision Tree
- Trained data using *decision tree* with default hyperparameter
- F1 score 0.65,0.59,0.00,0.00,0.50,0.89
- Accuracy: 0.61

4) Random Forest
- Trained data on logistic regression with hyperparameter max_iter=5000, solver=saga
- F1 score 0.62,0.73,0.33,0.00,0.67,0.84
- Accuracy: 0.69

## Conclusion

After training data on multiple algorithms. I came to conclusion that Random Forest understood the dataset best.
