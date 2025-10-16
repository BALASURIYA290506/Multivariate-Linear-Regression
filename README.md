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
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car (1).csv")
x = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:', regr.coef_)
print("Intercept:", regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:

<img width="809" height="79" alt="image" src="https://github.com/user-attachments/assets/714ce449-ead8-4406-8f83-509d72c6d8f8" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
