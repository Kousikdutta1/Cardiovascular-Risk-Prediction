# Cardiovascular Risk Prediction 

![1621618061250](https://user-images.githubusercontent.com/106880838/194716712-ba8cef0e-b972-499d-8756-478c061eaf30.jpg)
---
The heart is one of the main organs of the human body. The heart plays the most crucial role in the circulatory system. If the heart does not function properly then it will lead to serious health conditions including death. Cardiovascular diseases (CVDs) are the leading cause of death globally, according to WHO, an estimated 17.9 million people died from CVDs in 2019, accounting for 32% of all global fatalities. Though CVDs cannot be treated, predicting the risk of the disease and taking the necessary precautions and medications can help to avoid severe symptoms and in some cases, even death. As a result, it is critical that we accurately predict the risk of heart disease in order to avoid as many fatalities as possible.
The dataset provides the patients’ information. It includes 3390 records and 17 attributes. There are demographic, behavioural and medical risk factors. From that dataset we derived various insights that helped us know the weightage of each feature and how they are interrelated. The goal of this project is to develop a classification model that can predict if a patient is at risk of coronary heart disease (CHD) over the period of 10 years, based on demographic, lifestyle, and medical history.

# Summary :
Step 1 : First understanding the dataset, did some basic inspection on the raw data to check the number of columns also checked distribution of data and statistics of the data in each variable. I checked and dealt with missing values, Visualized the distributions and boxplots of each variable to handle the outliers, Cleaning the data. 

Step 2 : With the help of Exploratory Data Analysis I derived some meaningful results by doing univariate, bivariate and correlation analysis.

Step 3 : After EDA I went on to visualize the severity of multicollinearity. Removed multicollinearity based on VIF factor. Scaled the data and started experimenting different algorithms. 

Step 4 : I used seven Machine Learning models :  Logistic Regression, Decision Tree, Random Forest, XGBoost , K-Nearest Neighbors, Support Vector Machine and Naive Bayes. After training each model and tuning their hyper-parameters using grid search , I compared the performance of the models using different Evaluation Metrics.

# Result :
![gg](https://user-images.githubusercontent.com/106880838/194718072-461da461-1845-47ea-baa0-78e0373041f8.PNG)

# Conclusion :

Predicting the risk of coronary heart disease is critical for reducing fatalities caused by this disease, we can avert deaths by taking required medications and precautions if we can foresee the danger of this illness ahead of time.

* It is important to have a high recall score in this scenario because It is okay if the model incorrectly identifies a healthy person as a high risk patient, because it will not result in death, but if a high risk patient incorrectly identified as healthy, it may result in fatality. Support Vector Machine with rbf kernel is the best model with recall score of 0.88.

* There may be a case where the patients who are incorrectly classified as suffering from heart disease is equally important as patients who are correctly classified as suffering from heart disease, because patients who are incorrectly classified they may have some other illness, so in that case high f1 score is desired. Logistic Regression, XGBoost, K-NN these are the model with most F1 score.

* From our analysis, it is found that the 'Age' of the patient is the most important feature in determining the risk of coronary heart disease, middle and older age people are more prone to coronary heart disease than younger people followed by 'cigarettes per day', 'BP Meds', 'Prevalent Hypertension' are also very important feature in determining risk of heart disease.

* Future developments must include a strategy to improve models scores with the help of more data from people with different medical history.
