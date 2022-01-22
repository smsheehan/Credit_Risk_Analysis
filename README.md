# Credit_Risk_Analysis

## Overview of the analysis: 

The purpose of this analysis is to evaluate a variety of machine learning models against a dataset of information on credit card loans to see if we can accurately predict non-performing loans (NPLs).  Since the number of good (or high performing) loans greatly outnumber the non-performing loans we will need to evaluate models designed for unbalanced datasets such as this.  Before starting we should ground ourselves in an understanding of the issue and how our models might be useful in practice.  The following information can be found on statista.com at:  https://www.statista.com/statistics/211047/percentage-of-non-performing-loans-held-by-us-banks/#:~:text=In%202019%2C%200.89%20percent%20of,aftermath%20of%20the%20Financial%20Crisis.

![image](https://user-images.githubusercontent.com/90977689/150642820-839d263b-fdeb-47ab-9e42-b1bb9a848530.png)

As can be seen in the above blurb, it is important for us to understand that banks will use interest rate to help manage the risk.  Understanding this helps put into perspective how our model might fit into the big picture.  


## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

In this section, we will be evaluating six different machine learning models by evaluating their balanced accuracy, precision, and recall scores.  So it is important to explain each of these scores and what information they convey:
* Balanced Accuracy Score:
    Accuracy describes the percentage of predictions that are correct.  It is arrived at by the following formula: (True Positive + True Negative)/(True Positive + False Positive + False Negative + True Negative). However, this can be problematic when there is a large imbalance in the outcomes.  Balanced Accuracy takes into account both the true positive rate (sensitivity) and the true negative rate (specificity).  Balanced accuracy is derived by the following formula: (sensitivity + specificity)/2.
    
* Precision:
    Precision, also known as positive predictive value (PPV), is declaring how likely is a positive prediction likely to be a true positive.  It is found by taking the number of true positives and dividing by the sum of all positives (true positives and false positives).
    
* Recall scores:
    Recall is also known as sensitivity.  It is declaring how likely is it that my model will miss a true positive.  It is found by taking the number of true poistives and dividing by (true positives + false negatives)

### Models:

**Model 1: Naive Random Oversampling.**

![image](https://user-images.githubusercontent.com/90977689/150648657-1a41ccf6-cfa1-4775-be01-5cd238d12080.png)


This model has a balanced accuracy of 62.9%, a precision of 1 percent for high_risk loans, and a recall of 57% for high_risk loans.

**Model 2: SMOTE Oversampling.**

![image](https://user-images.githubusercontent.com/90977689/150646331-32ac4177-6838-4e40-b767-b954caa02380.png)

This model has a balanced accuracy of 62.8%, a precision of 1 percent for high_risk loans, and a recall of 62% for high_risk loans.

**Model 3: Undersampling with Cluster Centroids algorithm.**

![image](https://user-images.githubusercontent.com/90977689/150646395-f611f88e-d99b-4b00-9ecd-817a0eb20b40.png)

This model has a balanced accuracy of 53%, a precision of 1 percent for high_risk loans, and a recall of 61% for high_risk loans.

**Model 4: Combination over and under sampling with SMOTEENN.**

![image](https://user-images.githubusercontent.com/90977689/150646428-6cf50564-a40a-492e-84f8-aa5e523e6853.png)

This model has a balanced accuracy of 64.1%, a precision of 1 percent for high_risk loans, and a recall of 70% for high_risk loans.

**Model 5: Balanced Random Forest Classifier.**

![image](https://user-images.githubusercontent.com/90977689/150646480-d4296f61-eef2-4e61-a36f-c3b8d4b1069c.png)

This model has a balanced accuracy of 78.8%, a precision of 4 percent for high_risk loans, and a recall of 67% for high_risk loans.

**Model 6: Easy Ensemble AdaBoost Classifier.**

![image](https://user-images.githubusercontent.com/90977689/150646512-37e226b6-e3f9-41f4-9872-4ea8582bfacd.png)

This model has a balanced accuracy of 92.5%, a precision of 7 percent for high_risk loans, and a recall of 91% for high_risk loans.

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
