# CAD/HUF Currency Option Pricing Project

## 📚 Overview

This project focuses on the analysis and option pricing for the CAD/HUF (Canadian Dollar / Hungarian Forint) currency pair using financial time series modeling techniques.  
The study aims to:
- Analyze historical exchange rate data.
- Evaluate the statistical properties of log-returns.
- Estimate volatility (both historical and GARCH-based).
- Price At-The-Money (ATM) European Call and Put options.
- Compare multiple option pricing methods.

---

## 🛠️ Tools and Libraries Used

- Python 3.10+
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- statsmodels
- arch
- yfinance (for future improvements)

---

## 📈 Methodology

### 1. Data Preparation
- Imported CAD/HUF historical exchange rate data.
- Reconstructed closing prices using `Price` and `Change %`.
- Cleaned, sorted, and prepared the dataset for analysis.

### 2. Log-Returns Calculation
- Computed daily log-returns from the reconstructed prices.

### 3. Statistical Analysis
- Conducted visual normality checks (QQ Plot, Histogram).
- Applied formal statistical tests (Jarque-Bera, Kolmogorov-Smirnov, Anderson-Darling).
- Tested independence of log-returns using the Ljung-Box Test.

### 4. Volatility Estimation
- Calculated historical volatility (annualized).
- Modeled advanced volatility dynamics using a GARCH(1,1) model.

### 5. Option Pricing Models
- **Black-Scholes Model** (adjusted for FX options)
- **CRR Binomial Model**
- **Monte Carlo Simulation**

### 6. Comparison
- Compared Call and Put option prices from all three methods.

---

## 📊 Key Results

| Method          | Call Price | Put Price  |
|-----------------|------------|------------|
| Black-Scholes   | *value*     | *value*    |
| CRR Binomial    | *value*     | *value*    |
| Monte Carlo     | *value*     | *value*    |


- Predicted volatility using GARCH provided dynamic insights beyond historical estimation.

---

## 🚀 Advanced Extensions (Optional)

- Integration of Machine Learning models (Random Forest, XGBoost) for volatility forecasting.
- LSTM-based deep learning models for future return prediction.
- Real-time dynamic option pricing using updated data sources.

---

## 📂 Project Structure

```plaintext
CAD_HUF_Project/
├── CAD_HUF_Historical_Data.csv
├── CAD_HUF_Analysis.ipynb
├── README.md
└── requirements.txt
