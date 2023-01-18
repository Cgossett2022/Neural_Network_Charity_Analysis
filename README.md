# Neural_Network_Charity_Analysis

## Overview
For this project I used machine learning and neural networks to predict whether different charities will be successful if funded by our company, *Alphabet Soup*. In order to perform the analysis, I took the following steps: 1. Preprocess Data for a Neural Network Model 2. Compile, Train, and Evaluate the Model 3. Optimize the Model

## Results

### Preprocess Data
- I started by removing the EIN and NAME columns from the dataset.

- I established the "IS_SUCCESSFUL" column as the target variable.

- The additional columns: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" became my feature columns.

### Compile, Train, and Evaluate the Model
- My model contained two hidden layers with 80 and 30 neurons.

- The model's accruacy was below 75%, which did not achieve the target performance.

- In order to increase the target performance, I added a second model with two layers containing 100 and 30 neurons, and a third model with three layers containing 80, 30, and 10 neurons.

## Summary
The deep learning model reached an accuracy of around 73%, which is just below our target performance of 75% accruacy. 

### Recommendation
I would recommend using a random forest model since it could solve classification problems by sampling the data and building decision trees. 
