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

![nvo_classification_report](https://user-images.githubusercontent.com/96350388/166121623-7d0a2c14-7a8e-4feb-807b-8f2ea9d404a8.png)

### SMOTE Oversampling
- Balanced Accuracy Score: 0.6624

![SMOTE_classification_report](https://user-images.githubusercontent.com/96350388/166121631-9ffb2577-9bd8-452d-a21c-d8778dfa56e6.png)

### Undersampling
- Balanced Accuracy Score: 0.5447

![undersampling_classification_report](https://user-images.githubusercontent.com/96350388/166121639-58a7ee28-724b-4c6b-b1c4-22f24d7921b3.png)

### SMOTEENN
- Balanced Accuracy Score: 0.6707

![SMOTEENN_classification_report](https://user-images.githubusercontent.com/96350388/166121656-2c267e54-8227-491a-ab83-79efe9be21af.png)

### Balanced Random Forest Classifier
- Balanced Accuracy Score: 0.7824

![brfc_classification_report](https://user-images.githubusercontent.com/96350388/166121663-0f66f627-7d3b-4738-92ea-f53a761235eb.png)

### Easy Ensemble AdaBoost Classifier
- Balanced Accuracy Score: 0.9237

![eec_classification_report](https://user-images.githubusercontent.com/96350388/166121672-f012a0f0-8346-4b6a-b21e-29b0cef0fbf7.png)

# Summary
##### Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.





