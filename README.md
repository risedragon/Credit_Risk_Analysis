## Overview

Use different models of scikit-learn to predict credit risk, evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

I use 6 ways to predict RandomOverSampler. The performance shows bellow.

### Balanced Accuracy Score

Model|    algorithm       |Balanced Accuracy Score
-----|---------|-----------------------------------
LogisticRegression|RandomOverSampler|0.6398437216722869
..|SMOTE|0.6216172933512213
..|ClusterCentroids|0.5103309281216384
..|SMOTEENN|0.6357786318898034
BalancedRandomForestClassifier||0.7871246640962729
EasyEnsembleClassifier||0.9254565671948463

### Imbalanced classification report

RandomOversampler
![RandomOversampler](/images/RandomOversampler.png)

SMOTE
![SMOTE](/images/SMOTE.png)

ClusterCentroids
![ClusterCentroids](/images/ClusterCentroids.png)

SMOTEENN
![SMOTEENN](/images/SMOTEENN.png)

BalancedRandomForestClassifier
![BalancedRandomForestClassifier](/images/BalancedRandomForestClassifier.png)

EasyEnsembleClassifier
![EasyEnsembleClassifier](/images/EasyEnsembleClassifier.png)


## Summary

Preventing credit risk mainly lies in high-risk predictions. In this regard, each model has low prcision on high risk, also the f1 value of the models is also very low. Therefore, it is not recommended to use these models to predict credit risk.


