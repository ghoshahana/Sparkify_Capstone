# Sparkify_Capstone
This is an Udacity Data Science capstone Project. Here a fictitious company "Sparkify", aims to identify churns of the customers.
### Table of Contents

1. [Installation](#installation)
2. [Project_Motivation](#motivation)
3. [File Description](#files)
4. [Results](#results)
5. [Conclusion](#conclusion)

## Installation <a name="installation"></a>

Python 3 is required for this Project.*.

## Project Motivation<a name="motivation"></a>

Sparkify is a fictitious music company which provides free subscription to customers for a certain months. Post that the customer needs to renew his/her subscription. One who doesn't renew subscription is defined as a churn. This project aims to identify potential churned customers and features that might lead to churn. The underlined customer dataset is huge (12GB), so we would be using a subset of this dataset and Spark Machine Learning Models are to be used deal with Big Data. Exploratory Analysis would be done to find fruitful insights. Feature Engineering is to be used to create new additional features. Machine Learning models like Gradient Boost Classifier, Logistic Regression, Support Vector Machine and Random Forest are to be used to predict churn. Accuracy and F1-Score are the two metrics to be referred to select the best model. 

## File Descriptions <a name="files"></a>

Sparkify.ipynb is an iPython Notebook used for this project. 


## Results<a name="results"></a>

Gradient Boost Classifier, Logistic Regression, Support Vector Machine and Random Forest Classifiers are used to predict churn. Logistic Regression out-performed other models in terms of Accuracy and F1-Score. Grid Search along with Cross validation is used to tune the hyperparameters and further important variables are also identified. For details refer to the post [post](https://medium.com/@ghoshahana99/identify-customer-churn-594d8772286d)


## Conclusion<a name="conclusion"></a>

Our aim was to predict the churn of customer. Since the customer dataset is huge (12 GB) we used only a subset of the dataset. Big Data Tool Spark is used to deal with such a huge dataset. In the data exploration step, we removed duplicates in userid and missing userid. We also looked into the distribution of Subscription status across gender and payment status. Next step was Feature Engineering, where we created derived fields like Average file length per session, Session duration, Session count, the total subscription days, number of thumbs-up, number of thumbs-down, number of friend invitations, number of listened-to files per session. We created train data with 60% of obsevations and rest 40% are divided into two equal parts: crossvalidation and test. We used Gradient Boost Classifier, Logistic Regression, Support Vector Machine and RandomForest to predict the churn of customer. Logistic Regression out-performed other models in terms of accuracy and F1-Score. So, we used Grid Search along with Gradient Descent to fine tune the hyper-parameters and obtained an accuracy of 0.79 and F1-Score of 0.74. We also identified the variable of importance from the model like gender, add_friend, error, home, roll_advert, settings, mean_session_hr so that Sparkify can pay more attention to these features. Thus we were successful in predicting churn of customers.
