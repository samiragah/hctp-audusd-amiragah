# HCTP for AUD/USD

This repository contains the implementation of the Hybrid Candlestick Trend Predictor (HCTP) framework for the AUD/USD currency pair, as described in the research paper:

> "A Novel Multi-Timeframe Framework for EUR/USD: Integrating Neural Network Prediction and Candlestick Pattern Analysis"

The system combines:
- A Deep Learning Trend Predictor (DLTP) for weekly trend forecasts
- A rule-based Candlestick Pattern Recognizer System (CPRS) for daily signals in MQL4
- Multi-timeframe validation to align short-term patterns with long-term trends

The main architecture is based on the original HCTP framework for GBP/USD, with parameter recalibration for AUD/USD's volatility profile.

## Structure

- `/Python_Model`: DLTP training and prediction scripts (Python)
- `/MQL4_Codes`: CPRS and HCTP integration code (MQL4)
- `/Results`: Backtesting outputs and CSV files
- `/CSV_files`: CSV files

## Usage

1. Run `predict_trends.py` to generate weekly trend predictions.
2. Copy the output CSV to MetaTrader 4's `Files` folder.
3. Attach the `HCTP_EURUSD.ex4` expert advisor to the EURUSD D1 chart.

## License

MIT License - see LICENSE file for details.
