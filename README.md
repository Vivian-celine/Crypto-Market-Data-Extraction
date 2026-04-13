# 📊 Cryptocurrency Market Data Extraction & Analysis

**Author:** Vivian Celine
**GitHub:** [Vivian-celine](https://github.com/Vivian-celine)
**Data Source:** CoinGecko Public API
**Tools:** Python | Pandas | Requests | Matplotlib | Jupyter Notebook | Microsoft Excel

---

## 📁 Project Structure

```
crypto-market-data-extraction/
│
├── README.md
├── notebook/
│   └── crypto_extraction.ipynb        # Full Jupyter Notebook
├── data/
│   └── top10_crypto_2026-04-11.csv    # Top 10 coins dataset
├── historical_data/
│   └── Historical_price_2026-04-11.csv # Bitcoin 30-day price history
└── report/
    └── Report.docx                     # Written analysis report
```

---

## 🎯 Objective

To extract, clean and analyse live cryptocurrency market data from the CoinGecko 
public API — simulating a real-world client data extraction brief from a Nigerian 
fintech company (FinTrack Nigeria Limited).

The project answers 5 key business questions:
- Which coin has the highest market cap?
- Which coin gained or lost the most in 24 hours?
- What is the total global crypto market cap?
- What percentage does Bitcoin dominate the market?
- What trend is visible in Bitcoin's price over the last 30 days?

---

## 📡 API Endpoints Used

| Endpoint | URL | Purpose |
|---|---|---|
| Coin Market | api.coingecko.com/api/v3/coins/markets | Top 10 coins by market cap |
| Historical Price | api.coingecko.com/api/v3/coins/bitcoin/market_chart | Bitcoin 30-day price history |
| Global Summary | api.coingecko.com/api/v3/global | Global crypto market statistics |

---

## 🧹 Data Extraction & Cleaning Process

1. Imported requests and pandas libraries
2. Extracted data from all 3 API endpoints into DataFrames
3. Dropped 16 irrelevant columns out of 26 columns in coin market data
4. Checked for and confirmed no duplicate rows
5. Rounded all prices to 2 decimal places
6. Divided market cap by 1,000,000,000 and added B suffix to show values in billions
7. Split Unix timestamps in historical price data into readable date column
8. Dropped unnecessary Unix timestamp columns after splitting
9. Renamed columns for clarity after splitting
10. Converted price, volume and market cap columns to numeric data types
11. Divided historical market cap by 1,000,000,000 and rounded to 2 decimal places
12. Extracted total global market cap (USD) and Bitcoin market cap percentage from market summary dictionary
13. Formatted global market cap to billions with 2 decimal places
14. Rounded Bitcoin market cap percentage to 2 decimal places
15. Used Matplotlib to visualise Bitcoin price trend over 30 days
16. Exported both clean datasets as CSV files
17. Opened files in Microsoft Excel and used pivot tables to answer report questions

---

## 📊 Key Findings

1. **Bitcoin** had the highest market cap at **$1,453.89 Billion**
2. **Dogecoin** lost the most in 24 hours at **-1.41364%**
3. **USDC** gained the most in 24 hours at **+0.31854%**
4. **Total Global Crypto Market Cap:** $2,541.56 Billion
5. **Bitcoin Market Dominance:** 57.22%
6. **Bitcoin 30-Day Trend:** Peaked at $74,500 on March 17, declined sharply to $66,000 around March 29, then recovered toward $73,000 in early April — suggesting renewed buying interest

---

## 📈 Bitcoin 30-Day Price Chart

Bitcoin experienced a volatile 30-day period. The price peaked at approximately 
$74,500 on March 17 before declining sharply to a low of $66,000 around March 29. 
A recovery trend is visible from early April with prices climbing back toward 
$73,000, suggesting renewed buying interest.

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Python | Main programming language |
| Requests | Calling the CoinGecko API |
| Pandas | Data cleaning and manipulation |
| Matplotlib | Bitcoin price trend visualisation |
| Jupyter Notebook | Development and documentation |
| Microsoft Excel | Pivot tables for report answers |

---

## 📬 Contact

**Vivian Celine**
GitHub: [Vivian-celine](https://github.com/Vivian-celine)

---

*This project was built as a real-world API data extraction practice simulating 
a client brief from a Nigerian fintech company.*
