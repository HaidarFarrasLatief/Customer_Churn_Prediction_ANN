# Customer_Churn_Prediction_ANN

## Introduction

Customer Churn Prediction with Artificial Neural Network is my solution to make the algorithm that can predict when the customer stop buying a product (churn). I am using both Sequential and Functional Deep Learning Model with 2 times tuned model to evaluate more precise, which are:

1. Sequential Default, 100 epochs
2. Sequential Tuned 1, 100 epochs
3. Sequential Tuned 2, 50 epochs
4. Sequential Default, 100 epochs
5. Sequential Tuned 1, 100 epochs
6. Sequential Tuned 2, 50 epochs

*What differentiate between Default, Tuned 1, Tuned 2 are:

Default: Standard, without change or added optimizer, 100 epochs
Tuned 1: with optimizer, 0.0001 learning rate, 0.5 beta_1, 0.888 beta_2, 100 epochs
Tuned 2: same with Tuned 1 but with 50 epochs

Then I choose Deep Learning Model Tuned 2 with 50 epochs because it have the least gap between train and test accuracy which are 0.0027. 
That proved the deep learning is well enough. Eventhough there are the downside of this model, 
there are many false negative but the other model which are Functional Model are close enough in number. This false negative still significant enough to be a consideration in using this algorithm.

## Steps to Generate Model

1. Import Libraries & Data Loading
   
   I am using data from Keggle which can be downloaded from here:
   https://www.kaggle.com/datasets/blastchar/telco-customer-churn

   The dataset was made by BLASTCHAR on Keggle.

   The libraries I used are numpy, pandas, matplotlib.pyplot, seaborn, sklearn, tensorflow, keras, and time.
   
3. Data Cleaning
   There are unnecessary feature or column and Invalid data that I need to drop.
   
5. Exploratory Data Analysis (EDA)
   It is founded in EDA that the target feature/column (Churn) is not balance between values 'No' 
   (73,51%) and 'Yes' (26,49%), so I need to do make it more balance by running a downsampling  
   method in pre-processing part. The consideration to downsampling is because the ideal target 
   value percentage is beyond or near 30% (if only 2 values or boolean).
    
7. Data Pre-processing
   In pre-processing, the data are going through several modification and observation, which are 
   Handling Data Imbalance, Handling Outlier, Feature Selection, Scaling, and Encoding. in which I  
   will explain in more detail:

   7.1 Handling Data Imbalance
       

   7.2 Handling Outlier

   7.3 Feature Selection

   7.4 Scaling & Encoding
   
9. Deep Learning Modeling

## Model Conclusion
