# Stock Market Prediction System

A machine learning project that analyzes historical stock market data and predicts stock closing prices using regression models.

## Project Overview

The Stock Market Prediction System analyzes historical stock market data to understand price trends, trading volume, moving averages, and relationships between different stock features.

The project trains and compares multiple machine learning regression models to predict the **Closing Price** of the stock.

## Objectives

- Collect and prepare historical stock market data
- Clean and preprocess the dataset
- Analyze historical stock price and trading volume trends
- Calculate moving averages
- Analyze feature correlations
- Build stock price prediction models
- Compare model performance using evaluation metrics
- Visualize actual and predicted stock prices
- Present the analysis through a dashboard-style visualization

## Dataset

The project uses the **ZEUS** stock dataset from the Stock Market Dataset available on Kaggle.

Dataset source: :contentReference[oaicite:0]{index=0}

The dataset contains historical stock market information including:

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Trading Volume

The dataset used in this project contains **6,562 records**.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
Stock_Market_Prediction_System/
│
├── data/
│   └── ZEUS.csv
│
├── notebooks/
│   └── stock_market_prediction.ipynb
│
├── .gitignore
├── README.md
└── requirements.txt
