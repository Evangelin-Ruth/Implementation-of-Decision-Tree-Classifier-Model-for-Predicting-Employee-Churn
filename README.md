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
![image](https://user-images.githubusercontent.com/94219798/172996273-5a7f547b-b321-4c61-b76c-f0b11e00046d.png)
## data.info()
![image](https://user-images.githubusercontent.com/94219798/172996307-a3db7453-39ba-4a9a-9d1e-79baefe9a19c.png)
## data.head() using label encoder
![image](https://user-images.githubusercontent.com/94219798/172996352-cbcc82b3-7374-4d2b-99db-2b642b9f4860.png)
## x.head()
![image](https://user-images.githubusercontent.com/94219798/172996385-5641210e-9444-4662-aa38-58a8f5fb1110.png)
## accuracy
![image](https://user-images.githubusercontent.com/94219798/172996438-eaa73490-f292-42e0-8b49-889cf5a1a282.png)
## PREDICTION
![image](https://user-images.githubusercontent.com/94219798/172996463-381a39df-9092-460c-96de-ac4a7dab8111.png)



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
