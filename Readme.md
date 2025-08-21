# 📈 Fixed Income Order Management System (OMS)

## 🚀 Features

### 1️⃣ Market Watch
- Displays all available bonds (from `bonds.js`).
- Shows **Ticker, Bid/Ask, YTM, Current Yield, Face Value, Days to Maturity, Duration, Characteristics, Dates**.
- Prices **fluctuate randomly every few seconds** to mimic real markets.
- Clicking a bond auto-fills it in the Order Execution window.

### 2️⃣ Order Execution
- Place orders with full form:
  - **Side**: Buy / Sell
  - **Quantity**
  - **Order Type**: Market / Limit
  - **Limit Price** (mandatory if Limit)
  - **Stop Trigger** (for Stop orders)
  - **Time-in-Force**: GTC, IOC, DAY
- Supports:
  - **Market Order** → executes immediately at Bid/Ask.
  - **Limit Order** → executes only if price meets condition.
  - **Stop Trigger** → executes once trigger price is crossed.
- Orders can be **NEW, WORKING, FILLED, PARTIALLY_FILLED, CANCELLED, AMENDED**.

### 3️⃣ Trade Management
- Shows **Active Orders** with `Amend` and `Cancel` buttons.
- Shows **Executed Lots** (time, ticker, qty, price).
- Amend lets you update Qty/Price → order goes back to *WORKING* and can fill later.
- Cancel removes the order from the active queue.

### 4️⃣ Net Position
- Tracks open positions & performance.
- Supports **FIFO** and **LIFO** for average cost calculation.
- Shows:
  - Net Qty
  - Weighted Avg Cost
  - Market Price
  - **MTM (Mark-to-Market) PnL**
  - **Realized P/L** from closed trades
- Displays **Total MTM + Total Realized** at bottom.

---
## 📦 Installation

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/Fixed-Income-Website.git
   cd fixed-income-oms
    ```
2. open the html with live server