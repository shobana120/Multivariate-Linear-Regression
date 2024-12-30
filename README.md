# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.


### Step3
Get the value of X and y variables. 

### Step4
Create the linear regression model and fit.


### Step5
>Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube

### Step 6
Print the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
df.info()
df.head()
df.tail()
x =df[['weight',"volume']]
y =df['CO2']
regr =linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficents:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 =regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:

![WhatsApp Image 2024-12-29 at 12 20 19_e6aa0476](https://github.com/user-attachments/assets/86be5c3c-e3d0-49ac-9565-83d3efd327f6)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
