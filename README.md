# Credit_Risk_Analysis
#### Module 17 of Data Analytics Bootcamp

# Overview
The goal of this project is to apply machine learning to solve a real-world challenge: credit card risk.

I will employ different techniques to train and evaluate models with unbalanced classes. I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 

I then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Afterward, I evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.



# Results
#### Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

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
#### Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Due to our dataset's ratio of low risk to high risk loans being extremely unbalanced, non of these tests do well in every category. However, we can see that some of these tests are significantly better than others. The precision scores for almost all of these datasets are pretty meaningless, especially the precision regarding identifying low-risk loans. This is likely because of the sheer volume of low-risk loans compared to high-risk loans. The machine has far more examples to go off of when learning how to identify low-risk loans. The high-risk precision scores aren't as meaningless. We can tell with certainty that the ensemple classifiers both had better better precision with high-risk loan than all the resampling and SMOTEENN models. 

Ultimately, the recall and balanced accuracy scores tell us more about which test performed the best. As stated previously when discussing precision, the ensemble classifiers both were superior to the resampling and SMOTEENN models. Furthermore, the easy ensemble adaboost classifier outperformed all other models, including the other ensemble classifier, balanced random forest classifier. In order of balanced accuracy score from worst to best, the models performed as follows: undersampling (.5447), naive random oversampling (.6551), SMOTE (.6624), SMOTEENN (.6707), balanced random forest classifier (.7824), and easy ensemble adaboost classifier (.9237).

Knowing that recall tells you the ratio of true positives to all actual positives (meaning how close the model's predicted number of high/low-risk loans came to the actual number of high/low-risk loans), we could rank the models slightly differently. First and foremost, the easy ensemble adaboost classifier still outperformed all the other tests by far. However, the ranking of the other five models gets jumbled around a bit depending on if we are looking at high or low-risk loans. A chart with their rankings is below.

<img width="527" alt="Screen Shot 2022-04-30 at 2 23 44 PM" src="https://user-images.githubusercontent.com/96350388/166123174-ab2a5f34-8104-49d8-b2da-3b4a058c901c.png">

As can be seen from the chart, the easy ensemble adaboost classifier outperforms the rest in each category. As a result, I would recommend using this model for the most reliable predicitions. 




