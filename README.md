# Amazon-Stock-Prediction
Amazon Stock price prediction using RNN-LSTM
# Dataset
8 years of stock pricing data of Amazon is used for training. For testing purposes, past 1 year data is downloaded from yahoo Finance website everytime the program is run. Data is in CSV format. 
# Data Pre-processing
The dataset is converted to OHLC average (Open, High, Low, Closing prices) and added as a new column. This has been converted into two column time series data, 1st column consisting stock price of time t, and second column of time t+1. All values have been normalized between 0 and 1.
# Model
Model has 4 layers. 3 layers of LSTM is used to buil the RNN model using keras library, a dense layer is added. Linear activation function is used in the model.
# Training
Adam optimizer is used for convergence. 
# Testing
Test accuracy metrics is mean square error.
# Perdiction
Next day's stock price and last day's stock price predicted by the model are displayed.
# Conclusion
OHLC average is used as other two parameters (HLC average and closing value) are not that significant. The training and testing error rate is 11.42 and 46.69 which training has low rate than testing. The model can be improved more by optimizing it.

