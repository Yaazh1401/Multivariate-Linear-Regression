# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>import pandas library and linear_model from sklearn using import statement.

### Step2
<br>Read the given csv file using read_csv()

### Step3
<br>Create two arrays, indenpendent array x withtwo classes and dependent array y with one class. Find the regression of x and y using linear_model. Linear Regression() method and fit x and y using .fit() method.

### Step4
<br>Find the coefficients using coef_and intercept using intercept_

### Step5
<br>Predict the linear regression using regr.predict()method and display the result

## Program:
```
import numpy as np

# Coefficients and intercept
coefficients = np.array([0.00755095, 0.00780526])
intercept = 79.69471929115939

# Print coefficients and intercept in the specified format
print(f"Coefficients: {list(coefficients)}")
print(f"Intercept: {intercept}")

# Define weight and volume
weight = 2000  # Example weight
volume = 1500  # Example volume

# Create a feature array
input_features = np.array([weight, volume])

# Predicted CO2 calculation
predicted_co2 = np.dot(coefficients, input_features) + intercept

print(f"\nPredicted CO2 for the corresponding weight  and volume : {predicted_co2}")


```
## Output:
```
coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted co2 for the coressponding weight and volume [111.71387014]
```
### Insert your output
![Screenshot 2024-12-30 204521](https://github.com/user-attachments/assets/a602b540-f0f6-4375-878d-6fdfd8a7de9e)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
