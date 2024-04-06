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
4. calculate Mean square error,data prediction and r2.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: YUVARAJ B
RegisterNumber:  212222040186

import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data['Position']=le.fit_transform(data['Position'])
data.head()

x=data[['Position','Level']]
y=data['Salary']

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier()
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)

from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_predict)
mse

r2=metrics.r2_score(y_test,y_predict)
r2

dt.predict([[5,6]])

*/
```

## Output:


## Data.Head():

![Screenshot (81)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/1ae86723-fcaf-48e8-93ca-d420d85d7417)






## Data.info():

![Screenshot (82)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/679828bc-d267-49b6-ae37-83e1d765cb38)



## isnull() and sum():

![Screenshot (83)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/88caf551-9ff0-4cb9-b7c1-4b0f7866a7c3)




## Data.Head() for salary:

![Screenshot (84)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/3ac3b58e-25b0-4924-8e90-5e979cd1599e)




## MSE Value:
![Screenshot (85)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/c6d196d7-2b94-4014-a15f-82e5724c3874)






## r2 Value:

![Screenshot (86)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/236b4794-8ba5-43f6-8dcb-303e9e0c11f4)




## Data Prediction:

![Screenshot (87)](https://github.com/yashwanthrajadurai/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/128462316/30e0ed70-6481-4067-85b3-cd78d8990d5a)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
