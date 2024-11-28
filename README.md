# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

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
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
r2=metrics.r2_score(y_test,y_pred)
print("R2 score:",r2)
dt.predict([[5,6]])

/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Sudhindra.R
RegisterNumber: 24901168  
*/
```

##Output:

![Screenshot 2024-11-28 163218](https://github.com/user-attachments/assets/3fcfabde-e0d6-4313-b3d7-46d958877d33)

![Screenshot 2024-11-28 163236](https://github.com/user-attachments/assets/e2bb7524-37e4-4f70-a995-62dd59936940)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
