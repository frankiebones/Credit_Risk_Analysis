# Overview

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
