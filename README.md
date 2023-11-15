# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the libraries and read the data frame using pandas.
2. Calculate the null values present in the dataset and apply label encoder.
3. Determine test and training data set and apply decison tree regression in dataset.
4. Calculate Mean square error,data prediction and r2. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Elamaran S E
RegisterNumber: 212222230036

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
y=data[["Salary"]]
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]]) 
*/
```

## Output:
## Data.Head():
![279486017-17219e1b-9545-45e2-bb45-dd459016cbf9](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/ca2b98e5-f187-4108-8150-3ded90a3dd76)
## Data.info():
![279486035-6c499887-944a-476d-b365-f406cc541e6f](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/2939f832-4f9d-4275-b1ea-0b41307f6625)
## isnull() and sum():
![279486050-e97ab81f-f8b9-4813-83de-327da3214afe](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/a31ea00c-0ca5-4523-ba24-eb7bc35f75b3)
## Data.Head() for salary:
![279486068-ffc344dd-39b6-4370-9282-468f4642736c](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/7a6f6fe0-a70c-41c1-a495-91169607dd59)
## MSE Value:
![279486086-d063c559-f82f-4a52-b1fd-74c153c7d36e](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/8251952f-d8c2-47d0-abf0-750b0076dec4)
## r2 Value:
![279486100-2956ebf4-c1b2-4a45-9365-21f67717ebc4](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/75754e86-eb75-4366-a69d-606343f949bc)
## Data Prediction:
![279486119-516cbe0b-9937-4dd6-a5a8-1ac01a6673eb](https://github.com/elamarannn/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/113497531/55c1497f-75f6-4d1b-a74a-82cf7653592e)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
