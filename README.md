# Credit_Risk_Analysis-
# Module 18 Analysis
## Credit Risk Analysis 

## Overview of Analysis
In order to determine if a consumer/borrower is likely to comply with loan terms, or potentially default on a loan, analysis of previous loan information can be done.  This analysis can then be applied to future consumers/borrowers to determine the likelihood of their compliance with loan terms.  This project is designed to utilize several different techniques to train machine learning models and evaluate the results of t hose models.  This analysis is conducted on a known, provided dataset.  

## Analysis Results 
### Oversampling 
* Naive Random Oversampling 
    * Accuracy Score - 0.654260
    * Confusion Matrix - array([[   57,    30], [ 5934, 11184]], dtype=int64)
    * Imbalanced Classification Report (see below) 

* SMOTE Oversampling 
    * Accuracy Score - 0.651317
    * Confusion Matrix - array([[   56,    31],[ 5838, 11280]], dtype=int64)
    * Imbalanced Classification Report (See below) 

### Undersampling 
* ClusterCentroid Undersampling
    * Accuracy Score - 0.526346
    * Confusion Matrix - array([[  54,   33], [9723, 7395]], dtype=int64)
    * Imbalanced Classification Report (see below)

### Combined Over/Under Sampling
* SMOTEENN Sampling 
    * Accuracy Score - 0.637524
    * Confusion Matrix - array([[  61,   26], [7294, 9824]], dtype=int64)
    * Imbalanced Classification Report (see below)

### Ensemble Classification 
* Balanced Random Forest Classifier 
    * Accuracy Score - 0.906364
    * Confusion Matrix -array([[   58,    29],[ 1582, 15536]], dtype=int64)
    * Imbalanced Classificaiton Report (see below)

* Easy Ensemble AdaBoost Classifier
    * Accuracy Score - 0.942691
    * Confusion Matrix - array([[   79,     8],[  978, 16140]], dtype=int64)
    * Imbalaced Classification Report (see below) 

## Summary 
While results will vary between models, the Easy Ensemble AdaBoost classifier model used appears to be the most accurate learning model for the data we are analyizing.  The accuracy score is the highest of all models at 94.27%.  The precision of this model is 99.0% as well, which is the highest of all models run.  Based on this information, it can be assumed that results determined by this model are most likely to be accurate for the data being reviewed.  (Different datasets will require new analysis and review)
