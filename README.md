# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```

Program to implement the simple linear regression model for predicting the marks scored.
Developed by: padmasree.P
RegisterNumber:212225040293

import numpy as np
import pandas as pd
from sklearn.metrics import mean_absolute_error,mean_squared_error,r2_score
import matplotlib.pyplot as plt

df= pd.read_csv(r"C:\Users\acer\Downloads\student_scores.csv")
df.head(10)

plt.scatter(df['Hours'],df['Scores'])
plt.xlabel("Hours")
plt.ylabel("Scores")
x=df.iloc[:,0:1]
y=df.iloc[:,-1]
y_pred = lr.predict(x_test)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.linear_model import LinearRegression
lr=LinearRegression()
lr.fit(x_train,y_train)
lr.predict(x_test.iloc[0].values.reshape(1,1))
plt.scatter(df['Hours'],df['Scores'])
plt.xlabel('Hours')
plt.ylabel('Scores')
plt.plot(x_train,lr.predict(x_train),color='red')
lr.coef_
lr.intercept_
mse=mean_squared_error(y_test,y_pred)
rmse=np.sqrt(mse)
mae=mean_absolute_error(y_test,y_pred)
r2=r2_score(y_test,y_pred)
print("MSE:",mse)
print("RMSE:",rmse)
print("MAE:",mae)
print("R2:",r2)

```

## Output:
<img width="655" height="536" alt="WhatsApp Image 2026-04-29 at 10 00 14 AM" src="https://github.com/user-attachments/assets/0c45eaca-54cc-46c0-bb72-282cd18ddb5f" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
