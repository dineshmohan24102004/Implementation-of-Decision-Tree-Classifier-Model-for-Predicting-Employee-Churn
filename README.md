# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.import pandas module and import the required data set.

2.Find the null values and count them.

3.Count number of left values.

4.From sklearn import LabelEncoder to convert string values to numerical values.

5.From sklearn.model_selection import train_test_split.

6.Assign the train dataset and test dataset.

7.From sklearn.tree import DecisionTreeClassifier.

8.Use criteria as entropy.

9.From sklearn import metrics.

10.Find the accuracy of our model and predict the require values.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Dinesh.M
RegisterNumber:212222040039
import pandas as pd
data = pd.read_csv("Employee.csv")
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
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/8f135493-59e5-4131-a5ec-ff6880df26a4)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/bf654eca-276d-4ae4-a17c-4ba9d84a2da5)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/42eecd17-22b8-4848-8e59-a5131cbadfd7)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/efdc9c66-5a99-4610-92f0-d7efe6b39483)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/66181b82-b855-4878-a17d-bae2ffd3aedc)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/7ffa57c5-4104-4039-8002-7ec7f40b0ec0)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/071525b3-14db-492a-842f-6facd54fdf78)
![image](https://github.com/dineshmohan24102004/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119478475/9a24e2f5-01d4-452a-8887-955ea4842210)














## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
