# Phase 1 Project
![churn]("https://github.com/Eunice9521/Phase-3-Project/blob/main/Telcom%20Customer%20Churn%20Prediction.pdf")


## Project Overview
The aim of the project is to provide insight and come up with a model that predicts customer churn fot Telcom company. I will use the Telcom customer churn dataset to analyse and come up with insightful conclusions. Three Models will be used to train and predict data, the best performing model will be selected for future use to predict customer churn.

## Business Problem

Analyzing customer data in an attempt to understand and prevent customer churn is one of the top level priorities of any business. With constantly increasing competition in the telecommunications industry,it has become extremely difficult to secure customer loyalty. Telcom company is facing this challenge and would like to get more knowledge and understanding on the best way to maintain it's customer base as well as attract new customers on board. The secret to fighting churn is to dive deep into available data, discover trends and use the information to understand the customers and try to prevent them from moving to the competition.


## Data Understanding

Information is extracted from 'Telcom Customer Churn dataset'. The data was cleaned by checking and dealing with missing values, duplicates and checking the data types. The cleaned data was then used for the next processes of our project.
Some features were analyzed to help understand how they affect customer churn. The features analyzed were:
1. Voice mail plan.
2. International plan

From the above features, we laernt that:
1. Customers without a voice mail plan are more likely to churn as compared to those who have have subscribed to voice mail plan.

2. Most of the customers do not have an international plan. From the analysis, majority of the clients who have an international plan churn. This could be attributed to the clients not being citizens and are temporarily in the country.

A correlation heatmat was used to help understand how all the features correlated with churn.

![correlation heatmap]("C:/Users/Eunice Nduati/Desktop/download (2).png")


## Data Preparation

Before proceeding to the modeling stage, we needed to ensure that all categorical data is represented in a form that can be processed by machine learning algorithms. One commonly used technique for this is label encoding. Each category is given a unique numerical label, allowing machine learning algorithms to understand and process this information.

After examining the class distribution in the target column “churn”. The analysis results showed that there was a significant imbalance between the “Not Churn = 0” and “Churn = 1” classes.

Class imbalance in the target column “churn” is a situation where one class has a significantly higher frequency than another. This can affect the performance of the prediction model, especially when the minor class has important information.

The next step was consider suitable strategies to deal with class imbalance, such as SMOTE (Synthetic Minority Over-sampling Technique), an oversampling method used to handle class imbalance by creating synthetic samples for minor classes.



## Modeling

Three models were used to train and predict data. These are:

1. Logistic regression Model
2. Decision Tree Classifier Model
3. Random Forest Classifier Model


## Evaluation

The three models were evaluated for the accuracy and precision in predicting the test data. Random Forest model was found to successfully predict with an accuracy rate of about 92.04%. A confusion matrix was plotted to show the prediction.

![Confusion matrix]("C:/Users/Eunice Nduati/Desktop/download (3).png")

## Conclusion

Upon reviewing the results, the top four performing models in ranking from highest to lowest based on the provided metrics are:

1. Random Forest Classifier
Is ranked first among the models:

Precision Score: 0.90 Recall Score: 0.95 F1 Score: 0.92 Accuracy: 0.92 The Random Forest Classifier Model achieves a decent F1-score of 0.92. It shows a reasonable balance between precision and recall, indicating that the model can make accurate predictions while capturing a good proportion of positive cases. The overall accuracy of 0.92 suggests that the model performs well in classifying churn.

## Recommendations:
1. Use Random Forest Classifier for future prediction.
2. Encourage more customers to subscribe to voicemail plan.
3. Consider coverage outside the country to retain temporal customers from abroad.
