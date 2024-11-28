# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:MADHAN C 
RegisterNumber:24004329
import pandas as pd
from sklearn.tree import DecisionTreeClassifier,plot_tree
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotio
y=data["left"]
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
plt.figure(figsize=(8,6))
plot_tree(dt,feature_names=x.columns,class_names=['salary','left'],filled=True)
plt.show()
*/
```
## Output:
![decision tree classifier model](sam.png)
![Screenshot 2024-11-28 212746](https://github.com/user-attachments/assets/5d4a56bc-9de9-4abe-adcc-8a5631f10b09)
![Screenshot 2024-11-28 213038](https://github.com/user-attachments/assets/96df3b7a-6d74-4bb7-858c-b0c1e8e2e8d5)
![Screenshot 2024-11-28 213046](https://github.com/user-attachments/assets/df18601d-91c9-438e-b7a1-d0d90524efe1)
![Screenshot 2024-11-28 213050](https://github.com/user-attachments/assets/1b92e86b-d171-4a88-af88-42da48dba042)
![Screenshot 2024-11-28 213412](https://github.com/user-attachments/assets/43bc435c-bc82-4338-bfc5-a6f477de3479)
![Screenshot 2024-11-28 213447](https://github.com/user-attachments/assets/ffdd7d71-5fe4-485c-8988-97645a63ad30)
![Screenshot 2024-11-28 213536](https://github.com/user-attachments/assets/b51cee0a-faaa-42ca-952f-3d390b6dc6d5)
![Screenshot 2024-11-28 213652](https://github.com/user-attachments/assets/5607d1bf-a172-4984-ad99-6debc5c9d140)
## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
