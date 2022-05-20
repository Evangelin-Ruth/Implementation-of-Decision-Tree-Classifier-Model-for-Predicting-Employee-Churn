# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import pandas library to read csv or excel file.
2. Import LabelEncoder using sklearn.preprocessing library.
3. Transform the data's using LabelEncoder.
4. Import decision tree classifier from sklearn.tree library to predict the values.
5. Find accuracy.
6. Predict the values.
7. End of the program.
 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Evangelin.S
RegisterNumber: 212221230025
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```
## Output:
## data.head()
![image](https://user-images.githubusercontent.com/94219798/169461979-71ab14ec-08a9-4c76-b256-92a0217e4329.png)
## data.info()
![image](https://user-images.githubusercontent.com/94219798/169462170-f98bf4bb-dd6c-4554-adde-a2ae60bbc118.png)
## data.head() using label encoder
![image](https://user-images.githubusercontent.com/94219798/169462320-27fe40e5-213e-44f9-9989-ecac710edee7.png)
## x.head()
![image](https://user-images.githubusercontent.com/94219798/169462564-736475b3-dcf5-460a-b2e8-80cb4cc2cb2d.png)

## accuracy
![image](https://user-images.githubusercontent.com/94219798/169462705-c87352f2-b094-4990-8d0e-f370ffdd75fd.png)
## PREDICTION
![image](https://user-images.githubusercontent.com/94219798/169462825-3ba84c1c-9b34-4974-b075-81666ce8e390.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
