# Neural_Network_Charity_Analysis

## Overview
For this project I used machine learning and neural networks to predict whether different charities will be successful if funded by our company, *Alphabet Soup*. In order to perform the analysis, I took the following steps: 

1. Preprocess Data for a Neural Network Model 
2. Compile, Train, and Evaluate the Model 
3. Optimize the Model

## Results

### Preprocess Data
- I started by removing the EIN and NAME columns from the dataset.

<img width="1117" alt="remove_columns" src="https://user-images.githubusercontent.com/111243284/213302410-67ffb012-8b21-45b6-8978-16b745e9864e.png">

- I established the "IS_SUCCESSFUL" column as the target variable.

<img width="1082" alt="standard_scaler" src="https://user-images.githubusercontent.com/111243284/213302478-d3d728d2-adf6-4b02-82bb-33b2a605356c.png">

- The additional columns: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" became my feature columns.

<img width="975" alt="categorical_lists" src="https://user-images.githubusercontent.com/111243284/213302494-1fa8cad2-bb51-4e79-98a1-b993e2e7aac0.png">

### Compile, Train, and Evaluate the Model
- My model contained two hidden layers with 80 and 30 neurons.

<img width="882" alt="run_model" src="https://user-images.githubusercontent.com/111243284/213302798-7b323a9e-e013-4a9b-ba2e-b691e25c1a20.png">

- The model's accruacy was below 75%, which did not achieve the target performance.

<img width="598" alt="results_original" src="https://user-images.githubusercontent.com/111243284/213307854-faf9f7f5-47b7-463a-a667-6943fce12aea.png">

### Optimize the Model
1. In order to increase the target performance, I added a second model with two layers containing 100 and 30 neurons.

<img width="858" alt="model_2" src="https://user-images.githubusercontent.com/111243284/213302978-4ba31cd5-314d-4ff6-b8eb-aa1c41d6a0b7.png">

- The accuracy was 0.7313

<img width="915" alt="100-30_result" src="https://user-images.githubusercontent.com/111243284/213309601-190b48fa-aefe-4310-9457-96180ab1eb00.png">

2. I added a third model with three layers containing 80, 30, and 10 neurons.

<img width="858" alt="model_3" src="https://user-images.githubusercontent.com/111243284/213308997-dbb41a6c-6ce5-486d-bcf6-0061161c77f7.png">

- The accruacy was 0.7282

<img width="851" alt="results_2" src="https://user-images.githubusercontent.com/111243284/213310253-3ee36d59-ac3b-4919-9806-182e0cda6bb5.png">

## Summary
The deep learning model reached an accuracy of around 73%, which is just below our target performance of 75% accruacy.

- Model with two layers 80 and 30 neurons = accuracy of .7286
- Model with two layers 100 and 30 neurons = accuracy of .7313
- Model with three layers 80, 30, and 10 neurons = accuracy of .7282

### Recommendation
I would recommend using a random forest model since it could solve classification problems by sampling the data and building decision trees. 
