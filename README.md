# Bharat_Intern_Task_1
Taking an amazon company stock and  predicting its price by using LSTM. Use only Jupyter notebook code.

Step-1: Import Required Libraries:
Start by importing the necessary libraries for data analysis, visualization, and building the LSTM model.

Step-2:Download Stock Price Data:
Use the yf.download function from the Yahoo Finance library to download historical stock price data for Apple Inc. (AAPL).

Step-3:Data Preprocessing:
Extract the 'Close' prices from the downloaded data.
Normalize the data using MinMaxScaler to scale values between 0 and 1.
Split the data into training and testing sets.

Step-4:Create Sequences and Labels:
Define a function to create sequences and labels from the data. Sequences are input data for the LSTM model, and labels are the corresponding next-day prices.

Step-5:Build and Train the LSTM Model:
Create an LSTM model using Sequential from Keras. Compile the model with an optimizer and loss function, and then train it on the training sequences and labels.

Step-6:Make Predictions and Evaluate:
Use the trained LSTM model to predict stock prices on the test sequences. Inverse transform the predictions and labels to get the actual stock prices. Calculate the Mean Squared Error (MSE) to evaluate the model's performance.

Step-7:Visualize Results:
Plot the true and predicted stock prices to visualize how well the model performed.
