# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the pandas and scikit-learn libraries.

### Step2
Read the data from the csv file.

### Step3
Split the data into features (X) and target(y).

### Step4
Create and fit the linear linear regression model.

### Step5
Print the coefficients and intercepts of the linear regression model.

### Step6:
Make a prediction.

### Step7:
Print the predicted CO2 emissions.

### Step8:
End the Program.

## Program:
```
#Implementation of Multivariate Linear Regression
#Developed by: Jerowin Geo J A
#Register Number: 212223100016
import pandas as pd
from sklearn import linear_model
data = pd.read_csv("cars (1).csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercept",regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print("predicted CO2 for te corresponding weight and volume",predictCO2)
```
## Output:
![image](https://github.com/JerowinGeo/Multivariate-Linear-Regression/assets/147139744/f7dea23d-70dc-4d0b-b9b6-4b78a3825618)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
