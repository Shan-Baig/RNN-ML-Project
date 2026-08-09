# RNN Stock Price Prediction

A recurrent neural network (RNN) built from scratch to predict stock price movement, trained and tested on historical AAPL price data.

## Overview

This project explores how RNNs capture temporal patterns in sequential data — using daily stock price history as the case study. The model takes a windowed sequence of past prices and learns to predict the next value in the series.

## Approach

- **Data:** Historical daily AAPL price data (`AAPL.csv`)
- **Preprocessing:** Cleaned and normalized the raw price series, then reshaped it into sliding-window sequences suitable for RNN input (`preprocess.py`)
- **Model:** A recurrent neural network implemented in `rnn.py` / `model.py`, trained to predict the next time step from a sequence of prior prices
- **Experiment tracking:** Runs and hyperparameter results logged in `experiments_log_file.xlsx`

## How to Run

```bash
# 1. Clone the repo
git clone https://github.com/Shan-Baig/RNN-ML-Project.git
cd RNN-ML-Project

# 2. Install dependencies
pip install -r requirements.txt   # (add this file listing numpy, pandas, tensorflow/pytorch, etc.)

# 3. Preprocess the data
python preprocess.py

# 4. Train the model
python model.py
```

## Results

<!-- Fill in: e.g. final loss/RMSE, a plot of predicted vs. actual prices, or a short note on what worked/didn't -->
_Add a summary of model performance here — a loss curve or predicted-vs-actual chart makes this much more compelling to a reader._

## What I'd Improve Next

<!-- e.g. add attention mechanism, try LSTM/GRU variants, expand to multiple tickers, add train/val/test split details -->

## References

- [Recurrent Neural Networks (RNNs) — Towards Data Science](https://towardsdatascience.com/recurrent-neural-networks-rnns-3f06d7653a85)
- [Stock Market Predictions with RNN — Towards Data Science](https://towardsdatascience.com/stock-market-predictions-with-rnn-using-daily-market-variables-6f928c867fd2)
