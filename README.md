# 📈 Stock Market Dashboard

A **Streamlit-based dashboard** for tracking real-time stock market data using the [Yahoo Finance](https://finance.yahoo.com/) API via the `yfinance` library.

This app allows users to:
- Search and select a stock ticker
- View current market price, percentage change, and after-hours price
- See 52-week high and low prices
- Display live financial statistics in a clean, modern UI

---

## 🚀 Features

- 🔎 **Searchable Ticker Dropdown**:  Allows users to select a stock symbol from the list of available NASDAQ tickers. (e.g. AAPL, MSFT, TSLA)
- 📊 **Real-Time Market Summary** including:
  - Current Price
  - Daily Change (with %)
  - After-Hours Price
  - 52-Week High and Low
  - Volatility Metrics
- 📉 Color-coded price movements (green for gain, red for loss)
- 🕒 Time-stamped data display
- - **Financials & Actions**: Displays financial data and actions (e.g., dividends and stock splits).

## Setup

### Prerequisites
You need to have **Python 3.7+** installed. It is recommended to use a virtual environment to manage dependencies.

### Install Dependencies

1. Clone the repository or download the project files.
   
   ```bash
   git clone https://github.comKeerttna/stock-dashboard.git
   cd stock-dashboard
    ```
2. Create a virtual environment and activate it (optional but recommended):

   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

3. Install the requirements:

```bash
pip install -r requirements.txt
````

## Running the Dashboard
After installing the dependencies, you can run the Streamlit app:

``` bash
streamlit run stockDashboard.py
```
This will open the dashboard in your default web browser.


## 📁 Folder Structure

```
stock-dashboard/
│
├── stockDashboard.py        # Main Streamlit app file
├── nasdaq-listed.csv        # CSV file containing NASDAQ tickers
├── requirements.txt         # List of required Python packages
├── .gitignore               # Git ignore file
└── README.md                # Project documentation

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

