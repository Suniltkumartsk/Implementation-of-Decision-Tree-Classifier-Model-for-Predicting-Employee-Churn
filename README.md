# EXP6-Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required packages.
2.Read the data set.
3.Apply label encoder to the non-numerical column inoreder to convert into numerical values.
4.Determine training and test data set.   
5.Apply decision tree Classifier and get the values of accuracy and data prediction.
 
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: SUNIL KUMAR T
RegisterNumber: 212223240164
*/
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
print(data['left'].value_counts())
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data['salary']=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y = data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion = "entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])

```

## Output:
![Screenshot 2024-04-01 093316](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/c2d9e9d6-a6ed-4315-9701-b45bd1c7dd84)
![Screenshot 2024-04-01 093321](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/55f7ffa4-456e-49ac-855d-48dd4a119ec9)
![Screenshot 2024-04-01 093326](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/7ef64aae-e691-45bb-8362-60554469bd77)
![Screenshot 2024-04-01 093341](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/76e6b4ee-430b-4cd3-8c6d-67d0c3ad3ecb)
![Screenshot 2024-04-01 093405](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/f5856972-e329-4392-8ba5-3f90b72cbb0a)
![Screenshot 2024-04-01 093904](https://github.com/MOHAMEDAHSAN/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/139331378/b0b8136a-ef1c-4a62-9e1e-144d369d63ff)




## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
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
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: 
RegisterNumber:  
*/
```

## Output:
![decision tree classifier model](sam.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
