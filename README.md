# 📈 Stock Price Prediction System  
### 🧠 Corizo Machine Learning Internship – Minor Project  
**Author:** Sujith Kumar  

---

## 📌 Project Overview

This project aims to build a **Stock Price Prediction System** using **Long Short-Term Memory (LSTM)** neural networks. The model learns from historical stock closing prices and forecasts future values. The project demonstrates the use of deep learning for time series forecasting and financial data analysis.

---

## 🎯 Objective

- Use historical stock price data to train a deep learning model.
- Predict the future **closing prices** of Apple Inc. (AAPL) stock.
- Visualize model performance and compare actual vs. predicted prices.

---

## 🛠️ Technologies & Libraries

- Python 3.x  
- NumPy, Pandas  
- Matplotlib  
- Scikit-learn (MinMaxScaler, Mean Squared Error)  
- TensorFlow / Keras (LSTM, Dense, Dropout layers)

---

## 📁 Dataset

- **File:** `AAPL.csv`  
- **Source:** Yahoo Finance or any open financial market data platform  
- **Columns Used:**  
  - `Date` (timestamp of trading day)  
  - `Close` (closing price of the stock on that day)

---

## 🔍 Workflow

### 1. Data Preprocessing  
- Read and clean data  
- Convert date strings to datetime format  
- Normalize closing prices using MinMaxScaler  
- Prepare sequences of 60 days of data for training

### 2. Model Architecture  
A stacked LSTM model with:
- LSTM (50 units, return sequences=True)  
- Dropout (0.2)  
- LSTM (50 units, return sequences=False)  
- Dropout (0.2)  
- Dense layers (25 → 1)

### 3. Training  
- 80% training, 20% testing split  
- 20 epochs, batch size of 32  
- Loss: Mean Squared Error

### 4. Evaluation & Visualization  
- Compare predicted vs. actual prices  
- Plot results  
- Compute RMSE

---

## 📊 Result

- ✅ Model successfully predicts trends in stock prices  
- 📉 **Root Mean Squared Error (RMSE):** `3.35`

---

## 📈 Plot

![Actual vs Predicted Prices](#)  
> *Replace with image if hosted or use Jupyter to visualize the plot.*

---

## 📂 Folder Structure

```

Stock-Price-Prediction-System/
├── Stock-Price-Prediction-System.ipynb
├── AAPL.csv
├── requirements.txt
└── README.md

````

---

## ⚙️ How to Run

1. Clone the repository or download the files  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
``

3. Run the notebook:

   ```bash
   jupyter notebook Stock-Price-Prediction-System.ipynb
   ```

---

## 📬 Contact

**Sujith Kumar**
ML Intern @ Corizo
---

