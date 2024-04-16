# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

**Input:** 
Demographic data with the following features: 'country', 'year', 'uniqueid', 'bank_account', 'location_type',
       'cellphone_access', 'household_size', 'age_of_respondent',
       'gender_of_respondent', 'relationship_with_head', 'marital_status',
       'education_level', 'job_type' 

**Output:** Describe the output(s) of your model
Prediction if person has bank account

**Model Architecture:** Describe the model architecture you’ve used
XGBClassifier aith the following hyperparameters: min_child_weight=1, gamma=0.5, subsample=1.0, max_depth=3

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

The main performance metric is accuracy.
The model was train on 80% of data and tested on remainingf 20%.

Accuracy of the XGBoost model is 0.8895.

## Limitations

The model struggles with positive cases, as indicated by the relatively low True Positive rate (0.36) and high False Negative rate (0.64

## Trade-offs

The model's performance is stronger in recognizing negative cases but weaker in identifying positive cases, particularly with a notable number of false negatives.
