# Heart-Failure-Prediction-With-Fairness-ML

This project investigates fairness metrics of various classification models on the Heart Failure Prediction dataset on Kaggle using the FairLearn library. The attribute being investigated is gender, as the dataset is disproportionately male, and there is a misconception that men are more affected by heart disease than women. Four models (logistic regression, standard vector machine, decision tree, and random forest) were created to predict heart failure using all the features of the dataset. After constructing the model, fairness metrics were calculated using accuracy, precision, recall, f1 score, and the selection rate. Two bias reduction techniques were performed to see if fairness could be improved: demographic parity and equalized odds.    

## Data and Data Exploration 

The dataset for the project is listed in the data folder. Data exploration include graphs analyzing the distribution between men and women in all the features. Feature extraction was also performed to better understand which features may have more influence in the models 

## Fairlearn 

This folder holds all four models. Each model contains fairness metrics before and after bias mitigation. The bias reduction techniques include demographic parity and equalized odds for all models, and each are compared with accuracy, precision, recall, f1 score, and selection rate. 

### Citations 
[1] fedesoriano. (September 2021). Heart Failure Prediction Dataset. Retrieved December 5 from https://www.kaggle.com/fedesoriano/heart-failure-prediction. 
