## Credit Dataset Analysis Overview

This analysis concerns a dataset of various lending service information. The goal was to create a machine learning model that could be used to identify any credit risks from potential borrowers. 

I opted for a supervised learning method, where the 'loan_status' column was the 'key', and everything else was the info to train/test with. After creating the testing/training groups, I went with a Logistic Regression linear model. Logistic Regression seemed to apply the most to this case as all we're really trying to see is if someone is a risk or not. After fitting the model and generating some predictions, I created a quick confusion matrix and classification report to verify the results.

## Results Analysis

![credit_analysis_report](https://github.com/user-attachments/assets/9c0716c5-a7dd-4da8-9236-4ae2774a541a)


Overall, the model proved to be fairly accurate!

* Precision
    * When predicting users with no credit risk, the model was 100% accurate! However, the precision rate for determining users with high risk is down to 84%.

* Recall
    * The resulting rate for low risk clients is 99%. The high risk prediction result is 94%.

* Accuracy
    * The accuracy rate for low risk clients is 100%, with high risk client accuracy rate back down to 89%

## Credit Analysis Summary

Overall, I think the Logistic Regression model did a great job. When predicting low/no risk clients, the model was almost 100% accurate! Unfortunately, the predictions for high risk clients were a little less accurate with an average accuracy around 88-89%. This is potentially usable, but that would probably be something to check with the company in question. A potential reason for the lower high-risk scores is that there were much less high-risk entries in the dataset, so the model didn't have as many of those to learn from. That would probably be the best course of action for building off this model and improving the results. I would imagine indentifying high-risk loans would be the priority for a lending company, so improving the training dataset would likely give you an almost perfectly accurate model!

## Installation Instructions
* Clone repo to your local machine or just download the project files
* Open your code editing software of choice (Jupyter Notebook, VSCode, etc)
* Run the various cells at your discretion or run them all at once
