# Stock Market Prediction System

A machine learning project for analyzing historical stock market data and predicting stock closing prices using regression models.

## Project Overview

The Stock Market Prediction System analyzes historical stock market data to understand price trends, trading volume, moving averages, and relationships between stock market features.

The project also trains and evaluates multiple machine learning regression models to predict the **Closing Price** of the stock.

## Objectives

- Analyze historical stock market data
- Clean and preprocess the dataset
- Analyze historical price and trading volume trends
- Calculate moving averages
- Study correlations between stock market features
- Build machine learning models for stock price prediction
- Evaluate and compare model performance
- Compare actual and predicted stock prices
- Present the analysis using clear visualizations

## Dataset

This project uses the **ZEUS** stock market dataset from the Stock Market Dataset available on Kaggle.

**Dataset Source:** [Stock Market Dataset - Kaggle](https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset)

The dataset contains the following stock market features:

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Adjusted Close Price
- Trading Volume

For this project, the following features were selected:

- Date
- Open
- High
- Low
- Close
- Volume

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
```

## Project Workflow

### 1. Data Collection & Dataset Preparation

The historical ZEUS stock market dataset was loaded using Pandas.

The dataset contains historical information about:

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Trading Volume

### 2. Data Cleaning & Preprocessing

The dataset was checked for:

- Missing values
- Duplicate records
- Data formatting
- Required feature selection
- Feature scaling

The `Date` column was converted into datetime format.

The required numerical features were scaled using `StandardScaler`.

### 3. Exploratory Data Analysis

The following exploratory analysis was performed:

- Historical closing price trend
- Trading volume analysis
- 20-day moving average
- 50-day moving average
- Correlation heatmap

#### EDA Insights

- The ZEUS closing price shows significant fluctuations throughout the historical period.
- The stock experienced major price increases and decreases during different periods.
- Trading volume shows several sharp spikes, indicating periods of increased market activity.
- The 20-day moving average follows short-term price movements more closely.
- The 50-day moving average provides a smoother representation of the price trend.
- Open, High, Low, and Close prices show very strong positive correlations with each other.
- Trading Volume has a moderate positive correlation with the price-related features.

### 4. Stock Price Prediction Models

Three regression models were implemented:

1. Linear Regression
2. Decision Tree Regression
3. Random Forest Regression

The dataset was divided chronologically into:

- **80% Training Data**
- **20% Testing Data**

The target variable for prediction is the **Close Price**.

### 5. Model Training & Testing

Each model was trained using the historical training data and evaluated on the chronological test data.

Actual and predicted closing prices were compared using visualizations.

### 6. Performance Evaluation

The models were evaluated using the following metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Model Performance

| Model | MAE | MSE | RMSE | R² Score |
|---|---:|---:|---:|---:|
| Linear Regression | 0.192909 | 0.067297 | 0.259417 | 0.996924 |
| Decision Tree Regression | 0.294601 | 0.175266 | 0.418647 | 0.991990 |
| Random Forest Regression | 0.218725 | 0.091289 | 0.302141 | 0.995828 |

The metrics above represent the performance of the models on the project's chronological test dataset.

### 7. Data Visualization Dashboard

A dashboard-style visualization was created containing:

- Historical ZEUS closing price
- ZEUS trading volume
- Actual vs. Random Forest predicted closing prices
- Predicted closing prices from all implemented models

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/mohammadyousuf-63/Stock_Market_Prediction_System.git
```

### 2. Navigate to the Project Directory

```bash
cd Stock_Market_Prediction_System
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Virtual Environment

For Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 5. Install the Required Libraries

```bash
pip install -r requirements.txt
```

### 6. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the following notebook:

```text
notebooks/stock_market_prediction.ipynb
```

Run the notebook cells to reproduce the analysis, model training, evaluation, and visualizations.

## Project Scope

This project implements the required components of the Stock Market Prediction System:

- Data collection and preparation
- Data cleaning and preprocessing
- Exploratory data analysis
- Stock price prediction
- Machine learning model training and testing
- Model performance evaluation
- Data visualization dashboard

## Author

**Mohammad Yousuf**
