AI Stock Market Predictor 📈
An intelligent stock market analysis and prediction system using LSTM deep learning and machine learning algorithms to forecast Indian stock prices with interactive visualizations.

🌟 Features

📊 Advanced Price Prediction: LSTM-based deep learning model for accurate stock price forecasting
📈 Technical Analysis: Real-time RSI, MACD, Moving Averages, and Bollinger Bands
🎯 Trend Detection: Automated bullish/bearish market trend identification
📉 Risk Assessment: Volatility analysis and risk level evaluation
🖥️ Interactive Dashboard: Gradio-powered web interface for easy interaction
📱 Visual Analytics: Beautiful Plotly charts and comprehensive data visualizations
🔮 Multi-day Forecasting: Predict prices from 7 to 90 days ahead
⚡ Real-time Insights: Generate actionable market insights instantly

Installation
Usage
Features in Detail
Model Performance
Project Structure
Technical Indicators
Dataset
Technologies Used
Contributing
License
Disclaimer

🚀 Installation
Prerequisites

Python 3.8 or higher
pip package manager
4GB RAM minimum
GPU (optional, for faster training)

Step 1: Clone the Repository
bashgit clone https://github.com/Pranamya16/AI_StockMarketPredictor.git
cd AI_StockMarketPredictor
Step 2: Create Virtual Environment (Recommended)
bash# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python3 -m venv venv
source venv/bin/activate
Step 3: Install Dependencies
bashpip install -r requirements.txt
💻 Usage
Running the Jupyter Notebook
bashjupyter notebook stock_market_analysis_fixed_Version2_(1).ipynb
Quick Start

Load the dataset: Place your stock data CSV file in the project directory
Run all cells: Execute the notebook cells sequentially
Access the dashboard: The Gradio interface will launch automatically
Make predictions: Use the interactive sliders to predict future prices

Using the Gradio Interface
The system provides three main tabs:

🔮 Price Prediction

Select prediction timeframe (7-90 days)
View historical and predicted prices
Get price change percentages


📊 Technical Analysis

View current RSI, MACD, and volatility
Check market trend indicators
Analyze technical signals


💡 Key Insights

Overall performance metrics
Risk assessment
Market status and recommendations



🎨 Features in Detail
1. LSTM Deep Learning Model

Architecture: 3-layer LSTM with dropout regularization
Input Features: 11 technical indicators
Time Steps: 60-day historical window
Optimization: Adam optimizer with early stopping

2. Technical Indicators Calculated

Moving Averages: 7, 21, 50, 200-day MA
Exponential Moving Averages: 12, 26-day EMA
MACD: Moving Average Convergence Divergence
RSI: Relative Strength Index (14-day)
Bollinger Bands: 20-day with 2σ
Volatility: 21-day rolling standard deviation

3. Random Forest Model

Ensemble learning approach
100 decision trees
Feature importance analysis
Baseline comparison model

📊 Model Performance
LSTM Model Metrics
MetricTrainingTestingRMSE~0.35~0.37MAE~0.20~0.21R² Score~0.86~0.85
Random Forest Model Metrics
MetricTrainingTestingRMSE~0.85~1.00MAE~0.45~0.55R² Score~0.10-0.10
Note: LSTM significantly outperforms Random Forest for time-series prediction.
📁 Project Structure
AI_StockMarketPredictor/
├── stock_market_analysis_fixed_Version2_(1).ipynb  # Main notebook
├── 717503.BO.csv                                   # Stock dataset
├── requirements.txt                                # Dependencies
├── README.md                                       # This file
├── LICENSE                                         # MIT License
├── .gitignore                                      # Git ignore rules
├── CONTRIBUTING.md                                 # Contribution guidelines
📈 Technical Indicators
Trend Indicators

Moving Averages (MA): Identify trend direction
EMA: More weight to recent prices
MACD: Momentum and trend strength

Momentum Indicators

RSI: Overbought (>70) or Oversold (<30)
Signal Line: MACD crossover signals

Volatility Indicators

Bollinger Bands: Price volatility boundaries
Price Range: High-Low daily range
Historical Volatility: 21-day rolling std

📊 Dataset
Stock: 717503.BO (Bombay Stock Exchange)
Period: March 2014 - 2020
Records: 1,565 trading days
Features: Date, Open, High, Low, Close, Adjusted Close, Volume
Data Preprocessing

Date parsing and sorting
Missing value handling
Feature engineering (33 derived features)
Min-Max scaling (0-1 normalization)
Train-test split (80-20)

🛠️ Technologies Used
Core Libraries

Python 3.8+: Programming language
Pandas: Data manipulation
NumPy: Numerical computations
Matplotlib & Seaborn: Static visualizations
Plotly: Interactive charts

Machine Learning

TensorFlow/Keras: Deep learning framework
Scikit-learn: ML algorithms and metrics
LSTM Networks: Sequential prediction

Web Interface

Gradio: Interactive web dashboard
Jupyter Notebook: Development environment
