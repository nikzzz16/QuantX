# MarketPilot — Quantitative Multi-Asset Financial Intelligence & Backtesting Platform

A Streamlit hackathon implementation covering multi-asset analysis, quantitative indicators, correlation, strategy backtesting, realistic transaction costs, Buy & Hold benchmarking, robustness testing, regime analysis, stress testing, and a Featherless-powered AI Quant Analyst.

## Run

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

Create `.env`:

```env
FEATHERLESS_API_KEY=YOUR_NEW_KEY
FEATHERLESS_MODEL=Qwen/Qwen2.5-7B-Instruct
```

Never commit `.env` or share your API key.

Start:

```powershell
streamlit run frontend/app.py
```

## Included

- Gold, Bitcoin, NVIDIA historical data
- SMA / EMA, returns, annualized volatility, Sharpe, maximum drawdown
- Correlation matrix and rolling correlation
- SMA crossover, EMA trend, momentum, mean reversion
- Look-ahead-safe signal shifting
- Transaction costs and position sizing
- Strategy vs Buy & Hold
- Equity curves and entry/exit trade table
- Bull / bear / volatility regime analysis
- Parameter robustness heatmap
- Portfolio shock stress test
- Featherless AI Quant Analyst for explanation of calculated results
