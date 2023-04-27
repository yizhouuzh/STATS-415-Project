# STATS-415-Project
This is the final project of class STATS 415.
We chose an ongoing Kaggle competition [Novozymes Enzyme Stability Prediction](https://www.kaggle.com/competitions/novozymes-enzyme-stability-prediction).

The folder contains:

Code: 

Code_implementation_of_method_1.ipynb 
The code implementation of method 1. Including feature engineering, XGBoost models, and grid search.

Code_implementation_of_method_2.ipynb 
The code implementation of method 1. Including feature engineering, XGBoost models. Note that the parameters are tested and optimized manually and roughly.

grouping.ipynb
First, update the training dataset train.csv accoding to train_updates_20220929.csv.
Then generate 2 grouped datasets according to the first two strategies respectively.
The samples do not belong to any group will be deleted.

kaggle_grouping.ipynb
First, update the training dataset train.csv accoding to train_updates_20220929.csv.
Then comes the codes by R. Hatch, grouping with the third strategy.


Data: (.csv)

train.csv
The training dataset.

train_updates_20220929.csv
Some updates about the training dataset, inidicating which samples should be deleted or revised.

test.csv
The test dataset

grouped_sample_pH.csv
Group the training samples by only considering the similarities among the protein sequences, the first grouping strategy.

grouped_sample_no_pH_one_muta.csv 
Grouping, additionally requires that the samples in the same group should have the same pH values, and the number of mutations between the wildtype and a variant can only be one.

train_wildtype_groups.csv 
Divides each protein amino acid sequence into 3 parts evenly and makes global comparison, the third grouping strategy.
