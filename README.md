# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

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
Program to implement the SVM For Spam Mail Detection..
Developed by: S.THIRISAA
RegisterNumber:  212220040171

import pandas as pd
data=pd.read_csv("spam.csv",encoding='Windows=1252')
import chardet
file='spam.csv'
with open(file,'rb')as rawdata:
    result=chardet.detect(rawdata.read(100000))
result
data.info()
data.head()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,train_size=0.2,random_state=0)
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
![op1](op91.png)
![isnull](op92.png)
![predict](op93.png)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
