# Time-Based Tesla Stock Price Prediction

## About the Project

This project predicts the next day's closing price of Tesla (TSLA) stock using historical stock market data. The main objective was to understand how machine learning models can be applied to time-series financial data while following a complete machine learning workflow.

The project starts with collecting historical stock data from Yahoo Finance, followed by data cleaning, exploratory data analysis, feature engineering, model building, evaluation, and saving the best-performing model.

Instead of randomly splitting the dataset, a time-based train-test split is used to preserve the chronological order of the data and avoid data leakage.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- yFinance
- TA Library
- Joblib
- Jupyter Notebook

---

## Dataset

The dataset was collected directly from Yahoo Finance using the `yfinance` Python library.

The dataset contains daily stock market information, including:

- Date
- Open
- High
- Low
- Close
- Adjusted Close
- Volume

---

## Project Workflow

1. Download historical Tesla stock data.
2. Clean and preprocess the dataset.
3. Perform exploratory data analysis to understand stock trends.
4. Create technical indicators and additional features.
5. Split the data using a time-based approach.
6. Train multiple regression models.
7. Compare model performance.
8. Save the best-performing model for future predictions.

---

## Feature Engineering

To improve prediction performance, several additional features were created from the original stock data.

Some of the engineered features include:

- Lag Features
- Moving Averages (MA5, MA10, MA20, MA50)
- Exponential Moving Averages (EMA)
- RSI
- MACD
- Bollinger Bands
- Daily Return
- Log Return
- Rolling Standard Deviation
- Momentum
- Volatility
- Price Difference
- High-Low Difference

The target variable is the next day's closing price.

---

## Machine Learning Models

The following regression models were trained and compared:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

Random Forest was further improved using GridSearchCV with TimeSeriesSplit.

---

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The evaluation helped compare model performance and select the best-performing model.

---

## What I Learned

Working on this project helped me understand how machine learning can be applied to stock market data. I gained practical experience with data preprocessing, exploratory data analysis, feature engineering, time-series data handling, model training, hyperparameter tuning, and model evaluation.

It also strengthened my understanding of technical indicators such as RSI, MACD, Bollinger Bands, moving averages, and their role in financial data analysis.

---

## Future Improvements

Some improvements that can be made in the future include:

- Testing advanced models such as XGBoost and LightGBM
- Using LSTM or Transformer-based deep learning models
- Building a Streamlit web application for live predictions
- Integrating real-time stock prices using APIs
