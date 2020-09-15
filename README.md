# Crossvalidation_GridSearch_Classification
Cross Validation and Grid Search Automation for a Classification Problem
# Project Objective: How to apply cross validation and compare different models. 
   
    Please find below a summary of the overall approach.
    1. Chi-square test was performed to sigle out of the feature importance of the catagorical feature and it was concluded 
        that All catagorical features seems to have some kind of influence on the outcome.
    2. Following Features have been decided to be removed from model building and training as part of initial phase.
        -- Cabin : because most of the values (Aprox 70%) are missing
        -- Names:
        -- Ticket
    3. Model Accuracy has been tested with Cross validations score using following models.
          1.Decesion Trees Classifier
          2.RandomForest Classifier
          3.LogisticRegression
          4.Support Vector Classifier
          5.GradientBoosting Classifier
          6.XGBoost Classifier
          7.XGBoost Random Forest Classifier
    4. Based on 10 Crosss validation splits, it is found that the XGBoost Random Forest Classifier gave the better accuracy 
       score of Min Score of:75%, Maximum Score of:90% and Average Score of: 83%
    5. K-Fold Crosss validation was performed and extracted the best training and Testing sample out of 10 splits and 
       model was retrained.
    6. GridSearch Hyperparametr tuning approach was also tried to check if the model performance can further be increased.
## About Data
    The dataset has been taken from Kaggle Titanic Survivor_Prediction
