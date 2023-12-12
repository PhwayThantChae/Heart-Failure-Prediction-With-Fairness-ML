# Heart-Failure-Prediction-With-Fairness-ML

This project investigates fairness metrics of various classification models on the Heart Failure Prediction dataset on Kaggle using the FairLearn library. The attribute being investigated is gender, as the dataset is disproportionately male, and there is a misconception that men are more affected by heart disease than women. Three models (logistic regression, standard vector machine, and random forest) were created to predict heart failure using all the features of the dataset. After constructing the model, fairness metrics were calculated using accuracy, precision, recall, false positive rate, false negative rate, true positive rate, true negative rate, and selection rate. Two bias reduction techniques were performed to see if fairness could be improved: demographic parity and equalized odds.    

## Fairlearn 

This folder holds all three models -- logistic regression, svm, and random forest. Each model contains fairness metrics before and after bias mitigation. The bias reduction techniques include demographic parity and equalized odds for all models, and each are compared with accuracy, precision, recall, false positive rate, false negative rate, true positive rate, true negative rate, and selection rate. 

## Data and Data Exploration 

The dataset for the project is listed in the data folder. Data exploration include graphs analyzing the distribution between men and women in all the features. Additionally, a rudimentary analysis of the dataset with Fairlearn was also performed in the `Data_yl.ipynb` file. 

## Feature Importances 

To identify which features were most important in the dataset, lasso and ridge regression was performed in the `Feature_Importances_Heart_Disease.ipynb`. Feature importances were also extracted from a decision tree and random forest model in `Feature_Importances_Random_Forest_Decision_Tree.ipynb`. 

## Final Paper 

The final paper is the file: Final Paper -- Fairness in Heart Disease.pdf. All the citations for this project are included at the end of the paper. 

## Installation

Ensure you have Anaconda or Miniconda installed to manage the project environment and dependencies. If not, download Anaconda from [Anaconda's official website](https://www.anaconda.com/products/distribution) or Miniconda from [Miniconda's official website](https://docs.conda.io/en/latest/miniconda.html).

### Setting up a Conda Environment

Create and activate a Conda environment to manage the project dependencies separately:

```bash
# Create a Conda environment named 'heart_failure_env' with Python 3.9.7
conda create -n heart_failure_env python=3.9.7

# Activate the Conda environment
conda activate heart_failure_env
```

### Installing Required Packages

Install the necessary Python packages within the Conda environment:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn plotly fairlearn
```
