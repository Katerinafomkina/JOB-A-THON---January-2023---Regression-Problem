# JOB-A-THON---January-2023---Regression-Problem

<img width="1122" alt="Снимок экрана 2023-01-25 в 10 17 23" src="https://user-images.githubusercontent.com/8630013/214486186-9163fcb5-3c51-424f-8d04-54d1ef58d07d.png">


This is a repository to Jobathon January 2023 from [Analytics Vidhya]([https://datahack.analyticsvidhya.com/contest/dataverse-hack/True/#About](https://datahack.analyticsvidhya.com/contest/job-a-thon-january-2023/#About)


Problem Statement
VahanBima is one of the leading insurance companies in India. It provides motor vehicle insurances at best prices with 24/7 claim settlement. It offers different types of policies for both personal and commercial vehicles. It has established its brand across different regions in India.
Around 90% of the businesses today use personalized services. The company wants to launch different personalized experience programs for customers of VahanBima. The personalized experience can be dedicated resources for claim settlement, different kinds of services at doorstep, etc. Inorder to do so, they would like to segment the customers into different tiers based on their customer lifetime value (CLTV).
Inorder to do it, they would like to predict the customer lifetime value based on the activity and interaction of the customer with the platform. So, as a part of this challenge, your task at hand is to build a high performance and interpretable machine learning model to predict the CLTV based on the user and policy data.

•I did some EDA (check null values, check distributions, skewness, checked unique values, correlation)
I found that there was skewness in two numerical columns.
• Following that I cleaned data from outliers.
• Then I made baselines of following models: Linear regression, SGD, Random Forest, SVC, Ridge, Lasso, ELnet, XGB and checked which model is performing best. 
• Then, I trained all the models in 5-fold and 10-fold Cross-Validation.
• I found that XGB model is performing the best and I made hyperparametr tuning for it.
• After that I experimented various type of pre-processing: StandardScaler, Log-Transfoormation, Power-Transformation, RobustScaler(). I choose 
• Encoding technique – encoded with .get_dummies() 
• I tried use Ensemble technique: Lass0+SVR+XGB or Lasso+SVR+RF+XGB but i didn’t get a good score.
• My Final Model tuned XGB gave me on testing set: R2= 0.16212919350405086 and final score I got R2= 0.1537933031
