# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1 - import pandas as pd.

### Step2 - Read the csv file.

### Step3 - Get the value of X and y variables.

### Step4 - Create the linear regression model and fit.

### Step5 - Print the predicted output.

## Program:
```
DEVELOPED BY: DHARSHINI S
REG NO.: 212224100012

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print(predictedCO2)

```
## Output:

```
Coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
[114.75968007]
```
### Insert your output

<img width="1403" height="416" alt="image" src="https://github.com/user-attachments/assets/5099106c-2099-4503-9ba7-673291b7a2d9" />

<br>

### Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
