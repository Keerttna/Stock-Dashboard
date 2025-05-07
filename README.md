# 📈 Stock Market Dashboard

A **Streamlit-based dashboard** for tracking real-time stock market data using the [Yahoo Finance](https://finance.yahoo.com/) API via the `yfinance` library.

This app allows users to:
- Search and select a stock ticker
- View current market price, percentage change, and after-hours price
- See 52-week high and low prices
- Display live financial statistics in a clean, modern UI

---

## 🚀 Features

- 🔎 **Searchable Ticker Dropdown** (e.g. AAPL, MSFT, TSLA)
- 📊 **Real-Time Market Summary** including:
  - Current Price
  - Daily Change (with %)
  - After-Hours Price
  - 52-Week High and Low
- 📉 Color-coded price movements (green for gain, red for loss)
- 🕒 Time-stamped data display

---

## 📦 Requirements

Install the following dependencies:

```bash
pip install streamlit yfinance pandas
````

```bash
pip install numpy
```

---

## 🧑‍💻 How to Run

1. Clone this repository or copy the script.

2. Run the Streamlit app:

```bash
streamlit run stockDashboard.py
```

3. Open the local URL in your browser (typically `http://localhost:8501`).

---

## 📁 Folder Structure

```
stock-dashboard/
├── stockDashboard.py     # Main Streamlit app
├── nasdaq-listed.csv     # List of stock tickers for dropdown
├── README.md             # Project documentation
└── requirements.txt      # Package dependencies
```

---

## 🧠 Example Usage

```python
ticker = yf.Ticker("AAPL")
info = ticker.info
price = info["regularMarketPrice"]
```

Streamlit renders:

```
Apple Inc
196.94 USD
+2.66 (1.37%) today
Closed: 17 Apr, 7:59 pm • Disclaimer
After hours 197.25 +0.32 (0.16%)
```

---


## 📄 License

This project is licensed under the MIT License.

---

