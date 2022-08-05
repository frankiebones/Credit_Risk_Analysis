# Overview
In an effort to make data based decisions on whether to approve an individual for a line of credit we utilized numerous supervised machine learning models.<br>
We were supplied credit card credit data by LendingClub, a peer-to-peer lending services company.<br>
Upon inspection we were able to determine that this data was unbalanced, we have subsequently balanced it by utilizing multiple algorithms to resample the data.<br>

We used the following Python libraries: 
 - Pandas to separate the features from our target variable and familiarize ourselves with the data. 
 - Scikit-learn to create randomized training and testing datasets as well as reports to visualize and compare results. 
 - Imbalanced-learn to inspect different ways of balancing the dataset. 
 
# Results
- ### Balanced Accuracy Score
  - RandomOverSampler: **0.5755275247216383**
  - SMOTE: **0.5907065673475391**
  - ClusterCentroids: **0.49199736994644727**
  - SMOTEENN: **0.6121827037162187**
  - BalancedRandomForestClassifier: **0.7653921461981943**
  - EasyEnsembleClassifier: **0.9090692999101571**

- ### Precision
  - RandomOverSampler: **high risk 0.01 / low risk 0.99**
  - SMOTE: **high risk 0.01 / low risk 0.99**
  - ClusterCentroids: **high risk 0.00 / low risk 1.00**
  - SMOTEENN: **high risk 0.01 / low risk 1.00**
  - BalancedRandomForestClassifier: **high risk 0.03 / low risk 1.00**
  - EasyEnsembleClassifier: **high risk 0.09 / low risk 1.00**

- ### Recall
  - RandomOverSampler: **high risk 0.44 / low risk 0.71**
  - SMOTE: **high risk 0.53 / low risk 0.65**
  - ClusterCentroids: **high risk 0.54 / low risk 0.44**
  - SMOTEENN: **high risk 0.57 / low risk 0.66**
  - BalancedRandomForestClassifier: **high risk 0.62 / low risk 0.91**
  - EasyEnsembleClassifier: **high risk 0.86 / low risk 0.96**

![model_comparison](https://user-images.githubusercontent.com/15967377/182493726-214d34dd-8140-42fb-9031-582d52dcf0cf.PNG)
![ensemble_comparison](https://user-images.githubusercontent.com/15967377/182847063-a8aa8a04-09f7-438d-b0fd-ffd010a77578.PNG)

# Summary

As the F1 Score combines both the precision and recall of each model into a single metric it is highly useful when comparing classification models with imbalanced data. We can confidently say that based on the supplied data, the EasyEnsembleClassifier model would be best choice for predicting credit risk with a F1 score of ***0.97***. The BalancedRandomForestClassifier would be a close second at ***0.95***
