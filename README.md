# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd
### Step2
Read the csv file.
### Step3
Get the values of X and Y variable.
### Step4
Create the linear regression and fit.
### Step5
Predict CO2 with appropriate values.
### Step6
Display the predicted value.
## Program:
~~~
#Developed by :- K. Sai Eswar
#Register number:- 212221240020
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)
~~~
## Output:
<img width="828" alt="output" src="https://user-images.githubusercontent.com/93427011/154921321-1001b5f8-da72-4c0e-9059-283e1734324d.png">
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
