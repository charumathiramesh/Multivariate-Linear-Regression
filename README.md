# Implementation of Multivariate Linear Regression
## Aim:
### To write a python program to implement multivariate linear regression and predict the
output.
## Equipment’s required:
1. Hardware – PCs.
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner.
### Algorithm:
## Step1:
import pandas as pd.
## Step2:
Read the csv file.
## Step3:
Get the value of X and y variables.
## Step4:
Create the linear regression model and fit.
## Step5:
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm
cube.
## Step6:
Print the predicted output.
## Program:
```
Developed by: Charumathi.D
Reg.No: 22006878
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```

### Output:
## Insert your output:
![image](https://user-images.githubusercontent.com/119875375/214352963-5b6f7875-d7a6-4c19-a40a-2e1e438e4fee.png)


## Result:
Thus the multivariate linear regression is implemented and predicted the output using
python program.
