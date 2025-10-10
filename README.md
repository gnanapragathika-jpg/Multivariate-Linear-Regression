# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
1.Import the necessary libraries.
2.Read the dataset (carsemission.csv)
3.Select features (Weight, Volume) as X
4.Select target (CO2) as y
5.Create a Linear Regression model
6.Train the model using X and y
7.Obtain the model coefficients and intercept
8.Input new data for prediction (Weight, Volume)
9.Predict CO2 using the trained model
10.Output the predicted CO2 value
```
## Program:
```python
NAME: THEJASHREE S
REGNO: 212224240175

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)


```
## Output:

<img width="1170" height="84" alt="Screenshot 2025-10-10 094936" src="https://github.com/user-attachments/assets/66e527d5-d11c-4417-bac1-97f4dfb34cfc" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
