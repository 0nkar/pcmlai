# Stock Prediction Model

Stock Prediction Model is a Python project that uses a type of artificial intelligence called machine learning to predict the future price of a stock based on its past prices. It can help investors and analysts to understand how the stock market behaves and what factors influence the stock price. It can also help them to make better decisions about buying or selling stocks.

## Data
The data used for this project is the historical stock prices of Apple (AAPL), one of the most popular and valuable companies in the world. The data covers a period of five years from 2013 to 2018 and includes the daily closing prices of the stock. The data is obtained from Kaggle, a platform for data science and machine learning competitions and projects. The data source can be found here: https://www.kaggle.com/camnugent/sandp500

## Model
The model used for this project is a recurrent neural network (RNN) with a long short-term memory (LSTM) layer. A neural network is a machine learning technique that mimics the way the human brain works. A recurrent neural network is a type of neural network that can process sequential data, such as time series or text. A long short-term memory layer is a type of recurrent neural network that can remember long-term dependencies and avoid forgetting important information. This model is suitable for this project because it can capture the patterns and trends of the stock price over time and make accurate predictions.

## Hyperparameter optimization
A hyperparameter is a parameter that controls how the model learns from the data. For example, the number of hidden units, the number of layers, the learning rate, etc. Hyperparameter optimization is the process of finding the best combination of hyperparameters that can improve the model performance. For this project, I used trial and error to find the optimal hyperparameters. I tried different values for each hyperparameter and compared the results based on the mean squared error (MSE), which measures how close the predictions are to the actual values. The final hyperparameters are:

- Input size: 1
- Hidden size: 64
- Number of layers: 2
- Output size: 1
- Learning rate: 0.001
- Number of epochs: 100
- Window size: 20
- Dropout rate: 0.2
- Optimizer: Adam

## Results
The results of this project show that the model can predict the normalized closing price of AAPL with a reasonable accuracy. The model achieves a training loss of 0.0272 and a test loss of 0.2360 on the AAPL data, using MSE as the metric. The following plot shows the actual and predicted stock prices on the test set:

![Stock Price Prediction Plot](./images/s&p500.png)

We can see that the model can capture some of the general trends and fluctuations of the stock price, but it may not be able to predict sharp spikes or drops accurately. This is because the model only uses one feature (closing price) as the input, which may not capture the full complexity and dynamics of the stock market. Moreover, the model only uses data from one company (AAPL) and one index (S&P 500), which may not represent the diversity and variability of the stock market. Furthermore, the model only uses data from a specific time period (2013-2018), which may not reflect the current or future state of the stock market.

## Contact details
If you have any questions or feedback about this project, you can contact me at your-email@address.com or follow me on Twitter @your-username.
