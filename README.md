# Bitcoin Price Forecasting — MLP vs LSTM

A deep learning capstone project comparing two neural network architectures 
for next-day Bitcoin price prediction using 4+ years of daily market data.

## Overview
This project implements and compares a Multi-Layer Perceptron (MLP) and a 
Long Short-Term Memory (LSTM) network to forecast the next-day closing price 
of Bitcoin. The core question: does explicit sequence-awareness (LSTM) 
outperform an order-blind feedforward network (MLP) on volatile financial 
time-series data?

## Dataset
- Source: Bitcoin daily OHLCV data
- Period: January 2019 – August 2023
- Records: 1,674 daily entries
- Target: Next-day closing price (USD)
- Lookback window: 30 days

## Models
| Model | Architecture | Sequence-Aware |
|-------|-------------|----------------|
| MLP   | Feedforward neural network | ❌ |
| LSTM  | Recurrent neural network   | ✅ |

## Tech Stack
- Python
- PyTorch
- pandas, NumPy
- scikit-learn (MinMaxScaler, MSE/MAE)
- Matplotlib

- ## Project Structure
├── MLDL_CapstoneProject_AyeshaAmeen.ipynb  # Full notebook
├── Bitcoin_Daily.csv                        # Dataset
└── README.md

## How to Run
1. Clone the repo
2. Install dependencies: `pip install torch pandas numpy matplotlib scikit-learn`
3. Open the notebook in Jupyter or Google Colab
4. Run all cells top to bottom

## Key Results
Train/test split: 80% / 20% (chronological)
Evaluation metrics: MSE, MAE, RMSE
*(See notebook for full results and visualizations)*
