# rpg-coding-screen
Research Programming Group Coding Screen Challenge

#Setup:

1)	Clone the (empty) repo.
2)	Create a .gitignore file such that new contents in the data folder will not be tracked by git.  The data folder currently contains a single file.
3)	Download the data from (https://www.kaggle.com/ananta/credit-card-data/version/2) and extract into the data folder alongside the single file currently in that folder.  This will require creating a free Kaggle account if you don’t already have one.

#Task 1:

In either R or Python, write a function that takes as inputs:
1)  A transaction date range
2)	A customer age range
The function should produce a data frame with the count, mean, and standard deviation of the transaction amounts by card family and customer segment.  This should be limited to transactions during the date range from (A) and for customers within the age range from (B).  See emailed task list for example.

Call the function and print the results for age 28-44 and date May 10th - Jul 16th (inclusive) .

#Task 2:

In either R or Python, bring in the fraud flag from the *RAND_FraudBase.csv* file in the data folder of the git repo.  Use this file and *not* the FraudBase file from Kaggle.  Implement a logistic regression model to predict fraud.  As predictors, use transaction value, value as a share of limit (transaction value / credit limit), age, card family, customer segment, and transaction segment.  Fit the model using the full data without using cross validation.
Print a summary of the model and coefficients and briefly summarize the model.

#Task 3:

a.)	In either R or Python, implement a different classification algorithm of your choosing to predict fraud.  Use Transaction Value, Credit Limit, Age, and Card Family as features/predictors with 80/20 cross validation. Classify transactions as fraud if they have a greater than 0.25 (25%) predicted probability of being fraud.  Print relevant output and/or plots and a confusion matrix.  
b.)	Predict fraud using a logit model with the same predictors and cross validation as in (3a) above. Print relevant output and/or plots and a confusion matrix.  

#Task 4:

In writing:
a.)	Compare the models from Task 3 and explain which you might prefer in a production setting and why. And,
b.)	Imagine the credit card company has come up with a program designed to reduce fraud. Some cards are randomly assigned to be ‘treated’ with the anti-fraud program while others are not, and data is observed for both groups of cards. Briefly suggest a possible strategy for evaluating whether the program was effective.

#Submission:

Commit and push your submission to the git repo as a Jupyter notebook, R Markdown, or PDF.  Include the .r and .py scripts as well.  
