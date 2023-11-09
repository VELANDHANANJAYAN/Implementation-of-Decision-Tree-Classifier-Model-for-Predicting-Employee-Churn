# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas module and import the required data set.
2. Find the null values and count them.
3. Count number of left values.
4. From sklearn import LabelEncoder to convert string values to numerical values.
5. From sklearn.model_selection import train_test_split.
6. From sklearn import metrics.Find the accuracy of our model and predict the require values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Velan D
RegisterNumber:  212222040176

import pandas as pd
data = pd.read_csv("/content/Employee.csv")
data.head()
data.info()

data.isnull().sum()

data["left"].value_counts

from sklearn.preprocessing import LabelEncoder
le= LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()

x= data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]

x.head()
y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state = 100)


from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)

y_pred = dt.predict(x_test)
from sklearn import metrics

accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
1.DATASET:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/e93c01c7-cf39-4650-b80b-f8fc2d78b284)
2.df.inf0()
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/2e17d6d6-fe06-45b9-844f-19caf6376b02)
3.ISNULL:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/07fe46c6-545c-4476-8020-21c10917e447)
4.VALUE COUNTS:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/5d4b790c-9d52-4aed-9380-71c16d822955)
5.Dataset transformed head:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/ebc57a39-8df7-4f79-b81e-b61d12107c45)
6.X.head():
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/2000bb28-270b-4f3c-bbc0-5d297456e1e8)
7.ACCURACY:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/793ac355-bd48-4ed8-bc25-60b787a6f9e1)
8.PREDICT:
![image](https://github.com/VELANDHANANJAYAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119405038/82601c53-c7ca-499e-b312-0629e30d137d)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
