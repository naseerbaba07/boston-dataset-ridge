# Ridge Regularization (Ridge Regression)

This project demonstrates **Ridge Regression**, a regularization technique used to reduce overfitting in linear regression by adding an L2 penalty to the loss function.

## Files
- `boston.csv` – Dataset (synthetic Boston Housing–like data)
- `ridge_regression.py` – Python source code for Ridge Regression
- `requirements.txt` – Required Python libraries
- `README.md` – Project documentation

## Dataset
The dataset contains housing-related features and a target variable:
- **MEDV** – Median value of owner-occupied homes (target)

## How Ridge Regression Works
Ridge Regression minimizes:
```
Loss = RSS + α * Σ(w²)
```
where α controls the amount of regularization.

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the program:
   ```bash
   python ridge_regression.py
   ```

## Output
The script prints:
- Mean Squared Error (MSE)
- R² Score


## Additional Dataset Information

### Feature Description
| Feature | Description |
|---------|-------------|
| CRIM    | Per capita crime rate by town |
| ZN      | Proportion of residential land zoned for lots over 25,000 sq.ft |
| INDUS   | Proportion of non-retail business acres per town |
| CHAS    | Charles River dummy variable (1 if tract bounds river, else 0) |
| NOX     | Nitric oxides concentration |
| RM      | Average number of rooms per dwelling |
| AGE     | Proportion of owner-occupied units built prior to 1940 |
| DIS     | Weighted distances to employment centers |
| RAD     | Index of accessibility to radial highways |
| TAX     | Property tax rate |
| PTRATIO | Pupil–teacher ratio |
| B       | Proportion of Black population (derived feature) |
| LSTAT   | Percentage of lower status population |
| MEDV    | Median value of owner-occupied homes (Target) |

### Dataset Size
- Rows: **506**
- Columns: **14**

### Use Cases
- Demonstrating Ridge Regularization
- Handling multicollinearity
- Comparing Linear, Ridge, and Lasso regression models

### Disclaimer
This dataset is **synthetic** and intended strictly for educational and academic use.


### Algorithm: Ridge Regression

  1. Load the dataset from boston.csv

  2. Separate independent variables (X) and target variable (y)

  3. Split the dataset into training and testing sets

  4. Perform feature scaling using StandardScaler

  5. Initialize the Ridge Regression model with regularization parameter α

  6. Train the model using the training data

  7. Predict output values using the testing data

  8. Evaluate the model using:

            a. Mean Squared Error (MSE)

            b. R² Score

  9. Display the performance metrics