# Credit_Risk_Analysis
Columbia Engineering Bootcamp Module 17 - Supervised Machine Learning

## Analysis Overview
Jill and I are using the credit card credit dataset from LendingClub to predict credit risk among consumers. I am performing a varity of machine learning models and evaluating their performance to make a recommendation on whether or not these should be used to predict credit risk.

## Results

Naive Random Oversampling
![image](https://user-images.githubusercontent.com/92773195/154825841-e9175aac-20d6-4e5d-8b53-60e8f1ac4dc9.png)
![image](https://user-images.githubusercontent.com/92773195/154825853-58292a32-9010-48e9-82c8-c6b05b461c3c.png)

SMOTE Oversampling
![image](https://user-images.githubusercontent.com/92773195/154825859-9b3585ca-f239-4190-8df3-04940b96d860.png)
![image](https://user-images.githubusercontent.com/92773195/154825864-74e135eb-a090-4c2f-94c4-4314e5bef93e.png)

Undersampling
![image](https://user-images.githubusercontent.com/92773195/154825872-c16a8d87-dc81-4a29-9b21-a8424addb5a6.png)
![image](https://user-images.githubusercontent.com/92773195/154825877-c8d62583-bcc2-4650-a798-c1fafaba895a.png)

SMOTEEN Combination Under & Oversampling
![image](https://user-images.githubusercontent.com/92773195/154825888-fb4e35bb-cb62-474a-9276-9dcd834a57c6.png)
![image](https://user-images.githubusercontent.com/92773195/154825891-257ed765-d12f-477e-bf2a-dfbd156d332d.png)

Balanced Random Forest Classifier
![image](https://user-images.githubusercontent.com/92773195/154825905-aa37a7c9-9937-4a45-b6a7-a3b8feaf233c.png)
![image](https://user-images.githubusercontent.com/92773195/154825908-7177843e-e09b-4949-a55e-4427a0e1c985.png)

EasyEnsemble AdaBoost Classifier
![image](https://user-images.githubusercontent.com/92773195/154825920-537649cf-cf9d-499d-b536-fd05c9fe359d.png)
![image](https://user-images.githubusercontent.com/92773195/154825928-57e95393-de56-487a-831d-1c163432c0c3.png)


## Summary
Naive Random Oversampling has an accuracy score of 65.77% and a precision of 0.01

SMOTE Oversampling has an accuracy score of 62.9% and a precision of 0.01

Undersampling has an accuracy score of 52.9% and a precision of 0.01

SMOTEEN has an accuracy score of 63.8% and a precision of 0.01

Balanced Random Forest Classifier has an accuracy score of 79.6% and a precision of 0.04

EasyEnsemble AdaBoost Classifier has an accuracy score of 92.5% and a precision of 0.07

## RECOMMENDATION
Personally, I wouldn't recommend using ANY of these models as an accurate method of determining credit risk. While EasyEnsemble does have a 92.5% accuracy score, the precision metric of 0.07 as the highest precision of all the models indicates that these models are very poor at accurately predicting high risk creditors. The accuracy score appears to be very high because it is excellent at determining who is a LOW credit risk. However, the purpose of the model is to ensure that we can accurately classify high risk creditors, and with a precision of 0.07, the model is letting a lot of high risk creditors get through the system and classifying them as low risk instead which falsely inflates the accuracy score of the model. 
