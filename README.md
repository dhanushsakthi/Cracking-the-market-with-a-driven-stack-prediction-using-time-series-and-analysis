📈 Cracking the Market: A Driven Stack Prediction Using Time Series Analysis

This project explores the use of deep learning techniques, specifically **Long Short-Term Memory (LSTM)** networks, to forecast stock prices based on historical trends. Using Apple's (AAPL) historical stock data, we demonstrate how machine learning can be leveraged to decode the patterns in financial markets and make predictive insights.

---

### 🧠 Project Highlights

* Utilizes **LSTM** for time series prediction.
* Applies **MinMaxScaler** for data normalization.
* Employs a **60-day window** to predict the next day's closing stock price.
* Visualizes both actual vs. predicted stock prices.
* Evaluates model performance using **Mean Squared Error (MSE)**.

---

### 🗂 Dataset

* **Source**: [Yahoo Finance](https://finance.yahoo.com/)
* **Ticker Used**: `AAPL`
* **Features**: Date, Open, High, Low, Close, Adj Close, Volume
* **Used for Prediction**: `Close` price only

---

### 🛠️ Tech Stack

* Python 🐍
* Pandas, NumPy, Matplotlib 📊
* Scikit-learn 🧮
* Keras + TensorFlow 🔮

---

### 🔍 Methodology

1. **Data Preprocessing**:

   * Load and clean the dataset.
   * Normalize using `MinMaxScaler`.
   * Create sequences for LSTM input.

2. **Model Building**:

   * Stacked LSTM layers with dropout to prevent overfitting.
   * Output dense layer for prediction.

3. **Training**:

   * Trained over 10 epochs using an 80-20 train-test split.
   * Batch size: 32

4. **Evaluation**:

   * Plot loss curve and predictions vs actuals.
   * Compute MSE.

---

### 📊 Results

* The model captures general trends in the stock price.
* Demonstrates potential for further enhancement via hyperparameter tuning, external features (like volume, news sentiment), or longer training.

---

### 🚀 How to Run

```bash
git clone <your-repo-url>
cd <repo-folder>
pip install -r requirements.txt
jupyter notebook
```

Open the notebook file and run the cells sequentially.

---

### 📌 Future Improvements

* Integrate additional technical indicators (e.g., RSI, MACD).
* Incorporate news sentiment or social media data.
* Try other models (GRU, Transformer-based models).
* Real-time data feed integration.

---

### 👨‍💻 Author

**S. Dhanush**
