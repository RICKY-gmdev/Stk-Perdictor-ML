Overview

Forecasting stock prices is one of the most challenging tasks for financial analysts and researchers. Investors are highly interested in understanding the future direction of the stock market to make informed decisions.
This project aims to build a machine learning-based prediction system that forecasts the next day’s closing value of the Indian stock market index NIFTY 50.

Using historical market data and a deep learning model (LSTM), the system analyzes past patterns and predicts whether the market will go up or down tomorrow.

What This Project Does

✔ Downloads real-time historical NIFTY 50 data using yfinance

✔ Cleans and preprocesses the dataset

✔ Scales the numerical values for deep learning

✔ Creates 60-day sequences to train an LSTM model

✔ Trains a deep learning model to predict the next day’s closing price

✔ Compares the predicted close with yesterday’s close

✔ Provides a simple interpretation:

"NIFTY 50 will go UP tomorrow" or
"NIFTY 50 will go DOWN tomorrow"

Technologies Used:
  
  Python
  
  yfinance (to fetch live market data)
  
  NumPy & Pandas (data manipulation)
  
  Scikit-Learn (data scaling)
  
  TensorFlow / Keras (Deep Learning LSTM model)
  
  Matplotlib (visualization)

  Project Workflow
  
1️⃣ Data Collection

Fetch NIFTY 50 historical data from Yahoo Finance.

2️⃣ Data Preprocessing

Select required columns, handle missing values, and scale the data (0–1 range).

3️⃣ Sequence Creation

Use past 60 days of market data to predict the 61st day close.

4️⃣ Model Building

Create a deep learning model using:

2× LSTM layers

Dropout layers to prevent overfitting

Dense layers for final prediction

5️⃣ Model Training

Train on 80% of data, validate on 10%, test on the remaining 20%.

6️⃣ Prediction

Predict next-day closing price using the latest 60 days.

7️⃣ Market Direction Output

Compare predicted price with yesterday’s close and print:

UP or DOWN

📈 Results

The trained model produces:

A graph comparing actual vs predicted NIFTY closing values

A prediction for the next day

A clear message:
“The NIFTY 50 market will go UP tomorrow.”
or
“The NIFTY 50 market will go DOWN tomorrow.”

These outputs demonstrate the ability of LSTM models to learn temporal patterns in financial time-series data.
