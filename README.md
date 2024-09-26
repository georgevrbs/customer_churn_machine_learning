# Data used

The data used were found from IBM redirected from kaggle platform on the following link:

IBM link:
https://accelerator.ca.analytics.ibm.com/bi/?perspective=authoring&pathRef=.public_folders%2FIBM%2BAccelerator%2BCatalog%2FContent%2FDAT00148&id=i9710CF25EF75468D95FFFC7D57D45204&objRef=i9710CF25EF75468D95FFFC7D57D45204&action=run&format=HTML&cmPropStr=%7B%22id%22%3A%22i9710CF25EF75468D95FFFC7D57D45204%22%2C%22type%22%3A%22reportView%22%2C%22defaultName%22%3A%22DAT00148%22%2C%22permissions%22%3A%5B%22execute%22%2C%22read%22%2C%22traverse%22%5D%7D

Kaggle link:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

# Abstract

This paper aims to study different kinds of machine learning classification algorithms, 
on telecommunication customer data, in order to find the best algorithm that will identify 
if a customer will churn or not. In this way a telecommunication company could implement 
a way or strategy in order to reduce lost or decreasing revenue over time. The data were 
taken from kaggle platform, a well known site that provides data for machine learning 
projects, provided and in time updated by IBM company. The methodology used was to first 
visualize the data in order to get some first view and see if we could reduce, combine 
or transform the features that will help in the whole process later. Then standardization 
technique was used for numerical data as well as onehot encoding method for categorical 
data in order to be used by the algorithms properly. The data were split in training 
and test groups in percentage of 80-20 respectively. The algorithms used were Decision 
Tree, Logistic Regression, GaussianNB(Naive Bayes), Stochastic Gradient Descent, 
K-Nearest Neighbors and the ensembles Random Forest, Gradient Boosting Classifier, 
Extreme Gradient Boosting(XGBoost),  AdaBoost as well AdaBoost and Bagging on the 
first 4 simple algorithms. For feature selection the techniques used were SelectKBest 
and Recursive Feature Elimination with Cross-validation (RFECV). For the selection of 
model and hyperparameter tuning the GridSearchCV mainly on the simple models and 
RandomizedSearchCV for the ensemble models to decrease time of searching and fitting. 
At every point that cross-validation was needed the StratifiedKFold with 3, 5 folds was 
used because the percentage between the target classes were uneven. For the evaluation of 
models the metrics used were accuracy, f1-score and ROC AUC score. 


## Requirements

This project was run with python 3.10.9.

It is recommended to create a virtual environment if you want to run the project running below snippet in a shell:

```
python -m venv venv
```

Then activate the environment :
For linux based terminals:
```
.venv/Scripts/activate
```

To install the dependencies run:
```
pip install -r requirements.txt
```

Then open the .ipynb file in VSCode preferably and run the code
