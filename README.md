House prediction using ANN Model:
This is an active kaggle competition and I solve it by ANN(Artificial Neural Network).

Competition link : https://www.kaggle.com/competitions/house-prices-advancedregression-techniques/overview
Notebook link : https://www.kaggle.com/code/abirsaha123456/ann-model

1. Objective
The objective of this project was to predict home prices while training a deep learning
model using the House Prices: Advanced Regression Techniques dataset from Kaggle.
As we know that regression problem can be solved by the ANN algorithm. So in this project try to solve it by ANN and kaggle competition accept this one.

3. Data Preprocessing
To prepare the data for training, we followed these steps:
- Dropped the Id column.
- Missing values were imputed by taking the mean for numeric columns and the mode for
categorical ones.
- One-hot encoding was used for categorical variables.
- Features were standardized using StandardScaler to improve neural network
performance

3. ANN Architecture
The model consists of:
- Input Layer: 128 neurons, ReLU activation
- Hidden Layer 1: 64 neurons, ReLU activation
- Hidden Layer 2: 32 neurons, ReLU activation
- Output Layer: 1 neuron, linear activation (for regression)
Compiled with Adam optimizer, MSE loss function, and MAE as the evaluation metric.

4. Training Setup
 The data was divided into 70% training and 30% validation data.
 The model trained for 100 epochs using a batch size of 32.
 The validation data was used to monitor generalization or performance on
  previously untrained data.

5. Evaluation Results
The final evaluation on the validation set:
- Training MAE: 10,334
- Validation MAE: 23,709
- RMSE: ~37,842
- R² Score: ~0.87
The model shows good performance and generalization without major overfitting.

6. Prediction and Submission
The test dataset underwent the same processing steps, predictions were made, and
'submission.csv' containing the 'Id' and 'SalePrice' columns for submission to Kaggle was
generated and saved.
After submitting the csv file the public score was 0.41085 and the leaderboard position is 4259.
