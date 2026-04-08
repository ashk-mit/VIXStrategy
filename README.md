# VIXStrategy
SVXY / VIX Spike Backtest — Real Data + Visualization
======================================================
Pulls actual SVXY and VIX price history, finds every VIX spike
above a threshold since 2022, simulates entries/exits, and renders
a 5-panel dashboard saved as PNG.

Data sources:
  polygon  — free account at https://polygon.io
  alpaca   — free account at https://alpaca.markets
  yfinance — no key required (default, may rate-limit)

Usage:
  pip install requests pandas numpy matplotlib tabulate yfinance

  python svxy_vix_backtest.py                          # yfinance, default params
  python svxy_vix_backtest.py --source polygon --key KEY
  python svxy_vix_backtest.py --source alpaca  --key KEY --secret SECRET
  python svxy_vix_backtest.py --no-plot                # skip chart output
"""
