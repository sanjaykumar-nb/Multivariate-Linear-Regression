# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
 Import pandas.
### Step2
 Import linear model from sklearn.
### Step3
Read the files cars.csv.
### Step4
Assign he values for x and y as requried.
### Step5
Create the LinearRegression model and predict the output.
## Program:
```
#Developed by : SANJAYKUMAR N B
#Register Number : 212223230189

import pandas as pd
from sklearn import linear_model
data= pd.read_csv("car.csv")

X=data[['Weight','Volume']]
Y=data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)
```
## Output:
![alt text](<screenshot 2024-05-12.jpg>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.