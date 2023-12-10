# Heart-Failure-Prediction-With-Fairness-ML

This project investigates fairness metrics of various classification models on the Heart Failure Prediction dataset on Kaggle using the FairLearn library. The attribute being investigated is gender, as the dataset is disproportionately male, and there is a misconception that men are more affected by heart disease than women. Three models (logistic regression, standard vector machine, and random forest) were created to predict heart failure using all the features of the dataset. After constructing the model, fairness metrics were calculated using accuracy, precision, recall, false positive rate, false negative rate, true positive rate, true negative rate, and selection rate. Two bias reduction techniques were performed to see if fairness could be improved: demographic parity and equalized odds.    

## Fairlearn 

This folder holds all three models -- logistic regression, svm, and random forest. Each model contains fairness metrics before and after bias mitigation. The bias reduction techniques include demographic parity and equalized odds for all models, and each are compared with accuracy, precision, recall, false positive rate, false negative rate, true positive rate, true negative rate, and selection rate. 

## Data and Data Exploration 

The dataset for the project is listed in the data folder. Data exploration include graphs analyzing the distribution between men and women in all the features. Additionally, a rudimentary analysis of the dataset with Fairlearn was also performed in the Data_yl.ipynb file. 

## Feature Importances 

To identify which features were most important in the dataset, lasso and ridge regression was performed in the Feature_Importances_Heart_Disease.ipynb. Feature importances were also extracted from a decision tree and random forest model in Feature_Importances_Random_Forest_Decision_Tree.ipynb. 

### Citations 
[1] fedesoriano. (September 2021). Heart Failure Prediction Dataset. Retrieved December 5 from https://www.kaggle.com/fedesoriano/heart-failure-prediction. 
