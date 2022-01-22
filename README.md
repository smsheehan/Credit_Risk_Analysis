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

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
