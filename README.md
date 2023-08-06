## **Predict Customer Clicked Ads Classification by Using Machine Learning**

![Banner](banner.jpg)

***
### **Customer Type and Behaviour Analysis on Advertisement**

A Indonesian company wants to know the effectiveness of an advertisement that they serve, this is important for companies engaged in digital marketing consultants in order to know how much the advertisement is marketed so that it can attract customers to see advertisements.

***
### **Goal**
Improving marketing campaign performance and target the right customers to be able to clicked the ads.

***
### **Objective**
Create a machine learning model using supervised learning so that it makes easier for companies to make decisions.

***
### **Tools**
During this project I've use : <br>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) <br>
`as programming language` <br> <br>
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) <br>
`as notebook` <br> <br>
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white) <br>
`as IDE` <br> <br>
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) <br>
`as data preprocessing library` <br> <br>
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) <br>
`as data visualization library`

***
### **Contents**

***Dataset columns detail***

|   Feature |   Description |   Type    |
|-----------|---------------|-----------|
| Unnamed : 0    | ID Customer   | Numeric |
| Daily Time Spent on a Site    | Time spent by the user on a site in minutes| Numeric  |
| Age   | Customer' age in terms of years   | Numeric   |
| Area Income   | Average income of geographical area of costumer   | Numeric   |
| Daily Internet Usage  | Average minutes in a day customer on the internet  | Numeric   |
| Male  | Whether or not a customer was male    | Categorical   |
| Timestamp | Time which costumer clicked ads or closed window  | Categorical   |
| Clicked on Ad | Yes or No the customer clicked the ads    | Target Variable   |
| city  | City of the customer  | Categorical   |
| province  | Province of the customer  | Categorical   |
| category  | Category of ads   | Categorical   |

<br>

***Exploratory Data Analysis and Data Preprocessing***
On this section, there are few process such as :<br>
* handling missing values
* feature selection using *Univariate Analysis*, *Bivariate Analysis*, *Multivariate Analysis*
* feature encoding
* feature transformations to selected features using minmaxscaler.

***Data Modelling***
* Modeling using *KNeighborsClassifier*

***
### **Business Recommendation**

Based on machine learning modeling using *KNeighborsClassifier* method : 

* Accuracy: 0.94
* Precision: 0.9722222222222222
* Recall: 0.9090909090909091
* F1: 0.9395973154362416
* AUC: 0.9408468244084683

We have best 4th features for predicting the models againts the target `Clicked on Ad` :

* `Daily Internet Usage` : Time spent by the user on a site in minutes
* `Daily Spent Time on Site` : Average minutes in a day customer on the internet
* `Area Income` : Average income of geographical area of costumer
* `Age` : Customer' age in terms of years

***Actionable Insight***<br>
* Targeting the Ads to customers with high `Daily Internet Usage` and low `Daily Spent Time on Site`.
* Focusing the Ads to customers in 2 - 4 `Are Income` and on `Age` 40th - 60th years old. 
* Customers with high `Daily Spent Time on Site` have high chance to clicked ads.
* It's necessary to know about the reasons why the customers don't clicked the ads. Increase comfortable and convenience on website.
* We can broadcast promotions to customers with high `Daily Spent Time on Site`, so they are interested to clicked ads.


