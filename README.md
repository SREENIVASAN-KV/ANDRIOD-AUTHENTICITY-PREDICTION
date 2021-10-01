# ANDROID-AUTHENTICITY-PREDICTION
## Problem Statement and Data Summary ##

Android malwares is always a threat for the personal and professional data of users. This dataset consists of apps needed permissions during installation and run-time and related information. Data consist of apps from three different sources: google play, third-party apps and malware dataset. This file contains more than 30,000 Android apps features extracted at the time of installation and execution. Apps are collected from Google's play store, hiapk, app china, Android, mumayi , gfan slideme, and pandaapp. These .apk files collected from the last three years continuously. Here we are supposed to predict whether the app is benign(0) or malware(1).

## Approach ##

1)  familiarized and cleaned the data by doing preliminary analysis, and data pre-processing. Removed duplicates while keeping the class balance. 
2)  Filled null values using a datawig imputation model and standard procedures.
3)  performed EDA for understanding the relationship between variables.
4)  Used statistical tests and mathematical models for feature selection.
5)  One big challenge was tackling the text data and making it useful in the final modelling. We implemented an NlP classifier model on the text data with the help of TF-IDF vectorizer, PCA and XGBOOST. The result of the NLP model is used as a derived column in the final dataframe.
6)  Tried different classification models on the final dataframe and selected the one that came up with the optimum result. We got a very good classification report in XGBOOST with random searchCV.
7)  Used SHAP representation for model interpretability.
## Result ##
We built a classification model that predicts the malicious behaviour of android appls with an accuracy score of 89% and f1 scores of 0.84 and 0.92 for the benign and malware classes.
## Challenges ##
1) The data has 180+ columns, which makes the feature engineering and feature selection difficult.
2) Tackling the text data and making it useful in the final modelling.
## Future scopes ##
1) Deep learning using transformers(BERT,RoBERT etc).
2) Deploying the model on an android application.





