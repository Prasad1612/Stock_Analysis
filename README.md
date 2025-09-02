# 📈 Stock Price, Volume & Deliverables Dashboard  

An interactive **Streamlit dashboard** to analyze **NSE stock price, volume, deliverables, and trades** using the [nselib](https://pypi.org/project/nselib/) library.  
The app provides candlestick charts, deliverable vs intraday volumes, number of trades, and % deliverable trends — all with **quick date range filters** and **raw data view**.  

---

## 🚀 Features
- **Stock Symbol Selector** – Choose from NSE-listed stocks or enter manually.  
- **Quick Date Filters** – `1W`, `1M`, `6M`, `1Y`, or manual date range.  
- **Candlestick Chart** – Price movement with % change hover info.  
- **Deliverable vs Intraday Volumes** – Compare delivery vs intraday trades.  
- **Trades & % Deliverables** – Dual-axis bar & line chart.  
- **Raw Data Viewer** – Toggle to inspect clean historical data.  
- **Cache Management** – One-click clear cache button.  

---

## 🛠️ Installation  

Clone the repo and install dependencies:  

```bash
git clone https://github.com/your-username/Stock-Analysis-Dashboard.git
cd Stock-Analysis-Dashboard

pip install -r requirements.txt
```

---

## ▶️ Usage  

Run the Streamlit app:  

```bash
streamlit run Stock_Analysis.py
```

The dashboard will open in your browser (default: `http://localhost:8501`).  

---

## 📊 Example Output  

- **Candlestick chart** showing price movements.  
- **Stacked bar chart** for Deliverable vs Intraday volumes.  
- **Number of trades & % Deliverable** on dual axes.  

---

## 📂 Project Structure  

```
.
├── Stock_Analysis.py   # Main Streamlit app
├── README.md           # Documentation
└── requirements.txt    # Dependencies (optional)
```

Example `requirements.txt`:  

```
streamlit
nselib
pandas
plotly
kaleido
pandas_market_calendars
```

---

## ⚡ Notes
- Data is fetched from **NSE via nselib**. Availability depends on NSE API stability.  
- Only **EQ (Equity)** series data is used.  
- Numbers are formatted in **Indian units (K, L, Cr)** for readability.  

---

## 📜 License  

MIT License – free to use, modify, and share.  
