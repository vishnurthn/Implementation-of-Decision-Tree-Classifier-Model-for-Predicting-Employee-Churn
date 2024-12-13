# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

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
 data=pd.read_csv("Employee.csv")
 print("data.head():")
 data.head()
 print("data.info():")
 data.info()
 print("data.info():")
 data.info()
 print("data value countrs():")
 data["left"].value_counts()
 from sklearn.preprocessing import LabelEncoder
 le=LabelEncoder()
 print("data.head() for salary:")
 data["salary"]=le.fit_transform(data["salary"])
 data.head()
 print("x.head():")
 x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours",]]
 x.head()
 y=data["left"]
 from sklearn.model_selection import train_test_split
 x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
 from sklearn.tree import DecisionTreeClassifier
 dt=DecisionTreeClassifier(criterion="entropy")
 dt.fit(x_train,y_train)
 y_pred=dt.predict(x_test)
 print("Accuracy value:")
 from sklearn import metrics
 accuracy=metrics.accuracy_score(y_test,y_pred)
 accuracy
 print("Data prediction:")
 dt.predict([[0.5,260,0,2]])


/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Vishnurathan
RegisterNumber: 24001855
*/
```

## Output:

![image](https://github.com/user-attachments/assets/64e4bb0c-0a77-4e57-b146-7a3788757916)
![image](https://github.com/user-attachments/assets/ce400469-3c4b-4bd8-80ea-69e62566d835)
![image](https://github.com/user-attachments/assets/d625e6d4-44bd-4465-b3d3-00a97528ba8b)
![image](https://github.com/user-attachments/assets/f6328ecb-c8c1-4268-830e-0cb6e992b70f)






## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
