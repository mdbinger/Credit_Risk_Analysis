# Credit_Risk_Analysis
#### Module 17 of Data Analytics Bootcamp

# Overview
The goal of this project is to apply machine learning to solve a real-world challenge: credit card risk.

I will employ different techniques to train and evaluate models with unbalanced classes. I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 

I then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Afterward, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.



# Results
##### Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Naive Random Oversampling
- Balanced Accuracy Score: 0.6551
[insert screenshot of classification report]

### SMOTE Oversampling
- Balanced Accuracy Score: 0.6624
[insert screenshot of classification report]

### Undersampling
- Balanced Accuracy Score: 0.5447
[insert screenshot of classification report]

### SMOTEENN
- Balanced Accuracy Score: 0.6707
[insert screenshot of classification report]

### Balanced Random Forest Classifier
- Balanced Accuracy Score: 0.7824
[insert screenshot of classification report]

### Easy Ensemble AdaBoost Classifier
- Balanced Accuracy Score: 0.9237
[insert screenshot of classification report]

# Summary
##### Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.





