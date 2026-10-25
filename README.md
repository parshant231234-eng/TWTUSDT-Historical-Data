# TWTUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **TWTUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `TWTUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `70` months
- **Total Candles:** `3,018,127` 1-minute candles
- **Historical Range:** `2021-01-27 08:00:00` to `2026-10-24 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
TWTUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── TWTUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/TWTUSDT-Historical-Data/main/1m/2026/10/TWTUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
