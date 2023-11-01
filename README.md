# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import the necessary python packages using import statements.

2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().

3.Split the dataset using train_test_split.

4.Calculate Y_Pred and accuracy.

5.Print all the outputs.

6.End the Program.


## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by:S.Renuga 
RegisterNumber: 212222230118

import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values
y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)

y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
 
*/
```

## Output:

## data.head()

![Screenshot 2023-11-01 234608](https://github.com/RENUGASARAVANAN/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119292258/96d518b7-bba9-4022-bffa-ca4c508b7704)

 ## data.info()

![Screenshot 2023-11-01 234621](https://github.com/RENUGASARAVANAN/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119292258/707cb0d3-054f-4dde-ba16-b4b4c6acdd6f)

## data.isnull().sum()

![Screenshot 2023-11-01 234633](https://github.com/RENUGASARAVANAN/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119292258/f38a2557-b9bf-4d9d-b07a-2bd893d3a23c)


## Y_prediction value

![Screenshot 2023-11-01 234730](https://github.com/RENUGASARAVANAN/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119292258/96befbd9-4bed-4b02-ab73-9a6edb040825)

## Accuracy value

![Screenshot 2023-11-01 234754](https://github.com/RENUGASARAVANAN/Implementation-of-SVM-For-Spam-Mail-Detection/assets/119292258/795a18c6-5e9d-4a20-86b6-3056676901ee)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
