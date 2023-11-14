# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary packages using import statement.
2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().
3.Import KMeans and use for loop to cluster the data.
4.Predict the cluster and plot data graphs.
5.Print the outputs and end the program

## Program:

/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: VELAN D
RegisterNumber:  212222040176

import pandas as pd
import numpy as np
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
l=LabelEncoder()
data["salary"]=l.fit_transform(data["salary"])
data.head()
data["Departments "]=l.fit_transform(data["Departments "])
data.head()
data.info()
data.shape
x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','Departments ','salary']]
x.head()
x.shape
x.info()
y=data['left']
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
print("Accuracy = ",accuracy)
dt.predict([[0.5,0.8,9,260,6,0,1,2,1]])
*/


## Output:

Read csv file:

![280455798-60fbf767-4631-44d5-9926-2c24d3b628e2](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/c5981d3c-e076-4d1f-8170-b5027b954bd2)
Dataset info:

![280455808-c883f44b-7db1-4085-bd21-7fe0e5cf985d](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/a9a4491d-b8c5-408a-b580-ab8a150d451f)

![280455821-818d29c1-0319-4ad5-85bf-42e6b8ad4488](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/355d890f-3070-4bb2-8aff-a0329c977289)

Dataset Value count:

![280455848-79d18e09-70f9-470f-90d4-53c6a825af93](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/28691aab-9c76-407b-bfd3-a023d1f80314)

Dataset head:

![280455871-65a4703e-2083-45ec-81f4-463a1a302574](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/dea35cc3-f683-4490-9fbe-7d57716d3774)
Data info:

![280455902-0374428c-44d8-4a2c-a72a-6b3f2d820604](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/c3a2b541-280c-426e-9ca5-1e95988eda80)

Dataset shape:

![280455917-24970a9c-945c-4e0f-aeb2-fbdd4f82a8ee](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/4a213e0c-71b2-4de2-8d6c-17d6679c34fb)

![280455929-105592b3-78be-48dc-a29a-65f26ce957e5](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/a22ec751-2cbe-439f-a66a-dbba7dd1a37e)
Y-Pred:

![280455947-417f3652-06e2-4fa6-9d79-16dd29a2cec1](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/60e7adb8-7203-4b9d-af22-3727e2685352)

Accuracy:

![280455961-bedddd9e-cb40-4b59-9257-26e0afc28ae7](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/618af9e9-9b45-4784-947f-c9843c54d800)

Dataset Predict:

![280455976-a6d636e5-3a36-4016-b04b-b7a38512cae0](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/d2b85573-19fd-4632-9745-e6a7062bf592)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
