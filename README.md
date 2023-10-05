# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:
1.Import pandas as pd.
2.Obtain the information of the data.
3.Print the sum of null datas.
4.Using DecsionTreeClassifier imported from sklearn we get the accuracy.
5.Print the predicted values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SWETHA.S
RegisterNumber: 212222230155

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident",m"promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100
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
data.head() :

![Screenshot 2023-10-05 090810](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/1126aa2c-a35c-4373-a4b3-71918222222e)

data.info() :

![Screenshot 2023-10-05 093750](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/d3ff606f-4b33-488d-b2e6-b166edf9d196)

data.isnull().sum() :

![Screenshot 2023-10-05 091131](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/95603f90-13ee-4127-8084-14a33ff4191d)

Left column value count:

![Screenshot 2023-10-05 091237](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/1862bbdb-d561-462b-8b5a-ca127a681674)

data.head() for salary:

![Screenshot 2023-10-05 092101](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/f215aed6-42a9-42e3-b8fb-6c44ddb455fc)

x.head() :

![Screenshot 2023-10-05 092529](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/3f78c11f-2145-4e35-b879-ab35ca00ad9c)

Accuracy value:

![Screenshot 2023-10-05 094722](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/076986fa-23ff-4351-b293-1090a3c98858)

Data prediction:

![Screenshot 2023-10-05 094746](https://github.com/swethaselvarajm/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119525603/cc669c0e-6ba4-4794-b1a2-226dbb54289b)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
