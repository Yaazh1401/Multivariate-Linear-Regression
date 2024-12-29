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
import pandas as pd
from sklearn import linear_model
df =pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:',predictedCO2)


```
## Output:
```
coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted co2 for the coressponding weight and volume [111.71387014]
```
### Insert your output
![output img](<WhatsApp Image 2024-12-26 at 18.49.19_4feb1e82.jpg>)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.