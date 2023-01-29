# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas library as pd

### Step2
importing the dataset 

### Step3
extracting dependent and independent variables

### Step4
get the output


## Program:
```
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:

### Insert your output

![OUTPUT 10](https://user-images.githubusercontent.com/119478098/215322477-07b41402-5083-4418-b862-c5ca07fdec89.png)




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
