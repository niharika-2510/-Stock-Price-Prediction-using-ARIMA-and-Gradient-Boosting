# 📊 Stock Price Prediction using ARIMA and XGBoost

This project predicts future stock prices using **ARIMA** (for time series forecasting) and **XGBoost** (for non-linear modeling). The objective is to compare both models' performance and provide insights for data-driven trading strategies.

---

## 📌 Project Overview

This project implements two advanced models for stock price prediction:

- **ARIMA Model:** Captures linear trends and seasonality in time series data.
- **XGBoost Model:** Handles non-linear relationships using lagged features and rolling statistics.

---

## 💁️‍🎓 Project Structure

```
├── Model.ipynb              # Main Jupyter Notebook (Model Training & Evaluation)
├── data/                    # Dataset (or fetched from API)
├── outputs/                 # Model Predictions and Evaluation Outputs
├── README.md                # Project Documentation
└── requirements.txt         # Python Libraries and Dependencies
```

---

## 🔨 Setup Instructions

### 1️⃣ Clone the Repository:
```bash
git clone https://github.com/your-username/stock-price-prediction.git
cd stock-price-prediction
```

### 2️⃣ Set Up a Virtual Environment (Optional but Recommended):
```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies:
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Jupyter Notebook:
```bash
jupyter notebook Model.ipynb
```

---

## 📊 Models Implemented

### 1. ARIMA (AutoRegressive Integrated Moving Average)
- Captures linear patterns in time series data.
- Parameters `(p, d, q)` selected via Grid Search.
  
### 2. XGBoost (Extreme Gradient Boosting)
- Features include:
  - Lagged returns
  - Rolling mean and standard deviation
  - Volume changes
- Hyperparameters tuned using **GridSearchCV**.

---

## 📈 Performance Metrics

| Model      | RMSE     | MAE     | MAPE   |
|------------|----------|---------|--------|
| **ARIMA**  | 28.80    | 26.72   | 14.69% |
| **XGBoost**| 8.67     | 5.80    | 3.08%  |

---

## 📌 Key Insights
1. **Model Comparison**: XGBoost performed better in high-volatility periods.
2. **Hybrid Approach**: Combining both models may enhance prediction accuracy.
3. **Practical Use**: XGBoost for short-term predictions; ARIMA for long-term trends.

---

## 💄 Outputs
Find model outputs and evaluation plots in the `/outputs/` directory:
- Model performance comparison (ARIMA vs. XGBoost)
- Forecasted vs. Actual Stock Prices

---

## 📚 Dependencies

- Python 3.10+
- Jupyter Notebook
- Required Libraries:
    - pandas
    - numpy
    - matplotlib
    - seaborn
    - statsmodels
    - scikit-learn
    - xgboost
    - yfinance (for fetching stock data)

---

## 📤 Author

Niharika – B.Tech AIML Student

Feel free to reach out via https://www.linkedin.com/in/niharika-dhingra-a3440824a/

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

