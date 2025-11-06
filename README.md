# Natural Gas Short-Term Extrapolation — 20-Day Forecast Demo (Spline)

## Overview
Extends the spline-fitted forward curve to project short-horizon prices (e.g., next 20 days) and visualizes the trajectory vs. latest historical points.

## Data
- Uses the same `Nat_Gas.csv` (dates + price).
- Preprocess: datetime conversion, sorting.

## Methods
- `UnivariateSpline` fit on historical prices
- Generate future date range (e.g., 20 days) and compute projected prices
- Line plot for quick inspection

## Results
- Future 20-day price path (illustrative)
- Visual comparison with recent history

## Notes & Limitations
- This is a **demo extrapolation**; not a trading model.
- No seasonality/exogenous features included.
- Validate via backtests before any use.

## Next Steps
- Add rolling-origin backtest
- Confidence bands via residual variance
- Compare with ARIMA/Prophet/GBM baselines
