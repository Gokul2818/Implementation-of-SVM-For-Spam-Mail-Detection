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
Developed by: GOKUL S
RegisterNumber:  24004336
import chardet
file='spam.csv'
with open (file,'rb') as rawdata:
    result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("spam.csv",encoding='windows-1252')

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
Encoding:

![Screenshot 2024-12-25 223948](https://github.com/user-attachments/assets/7e8c7a91-4f4d-4da3-bf41-43ee564ed2aa)

Head():

![Screenshot 2024-12-25 224359](https://github.com/user-attachments/assets/7900afb0-1530-4c8a-aec5-6a574ccb8aca)

Info():

![Screenshot 2024-12-25 224034](https://github.com/user-attachments/assets/6f43b5bb-a7df-4ef5-8356-97713d650f77)

Isnull().sum():

![Screenshot 2024-12-25 224011](https://github.com/user-attachments/assets/dad51204-e488-49da-8983-47a21095ff77)

Prediction of y:

![Screenshot 2024-12-25 224103](https://github.com/user-attachments/assets/bee3fb36-c4d5-4b56-b048-827fb824febc)

Accuracy:

![Screenshot 2024-12-25 224115](https://github.com/user-attachments/assets/9130f12c-42a7-4381-81fe-abfefba7ffe4)
## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
