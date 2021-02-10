# LTFS Hackathon - Upsell Prediction

## Problem:
LTFS Hackathon challenged its participants to predict if the borrower will top up his loan during his loan tenure. If yes, the participants had to predict the timeline the top up bucket. In particular, there were 7 buckets for prediction - No Top-Up Service, 12-18 Months, 18-24 Months, 24-30 Months, 30-36 Months, 36-48 Months and >48 Months. I use the seminal [XGBoost model](https://xgboost.readthedocs.io/en/latest/index.html) to make these predictions. 

## Contents: 
1. 'Test' and 'Train' directories contain data dictionary, demographic data and bureau data. All of these files were received from LTFS. 'bureau_cleandata.csv' contains bureau data rolled up to the ID (unique identifier) level.

2. 'data_clean_test.ipynb' and 'data_clean_train.ipynb' are python codes used to process the data from LTFS. 

2. 'final_dataset' directory contains data received post data processing using 'data_clean_test.ipynb' and 'data_clean_train.ipynb' codes.

3. 'Model_1.ipynb' predicts the target variable (Top-Up Month) using XGBoost model. It uses data from the 'final_dataset' directory.  

3. 'submissions' directory contains the submissions template and various submission iterations submitted to assess the model on test data.   