# FINANCIAL INCLUSION IN AFRICA 


## OVERVIEW
Financial inclusion remains one of the main obstacles to economic and human development in Africa. Across Kenya, Rwanda, Tanzania, and Uganda only 9.1 million adults (or 14% of adults) have access to or use a commercial bank account. Traditionally, access to bank accounts has been regarded as an indicator of financial inclusion. Access to bank accounts enable households to save and make payments while also helping businesses build up their credit-worthiness and improve their access to loans, insurance, and related services. Therefore, access to bank accounts is an essential contributor to long-term economic growth.

The objective of this project is to create a machine learning model to predict which individuals are most likely to have a bank account. The model and solution could provide an indication of the state of financial inclusion in Kenya, Rwanda, Tanzania and Uganda, while providing insights into some of the key factors driving individuals’ financial security.

The developed model should predict the likelihood of the person having a bank account or not (Yes = 1, No = 0), for each unique id in the test dataset.
 
## DATA
The dataset contains demographic and financial services information of approximately 33,600 individuals from four African countries - Kenya, Rwanda, Tanzania, and Uganda.

## MODEL 
The final model I decid eto use is XGBoost model. The model has highest accuracy of all experimented models (0.8895)

## HYPERPARAMETER OPTIMSATION
I chose to use Grid Search to optimise XGBoost parameters.
Parameters: min_child_weight=1, gamma=0.5, subsample=1.0, max_depth=3

## RESULTS
Model's accuracy is 0.8895 and is acceptable. The model performs well in identifying negative cases, as evidenced by the high True Negative rate (0.98), but the label is unbalanced - 86% of data are negative cases (doesn't have bank account).
The model struggles with positive cases, as indicated by the relatively low True Positive rate (0.36) and high False Negative rate (0.64).

## (OPTIONAL: CONTACT DETAILS)
n/a
