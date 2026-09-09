# FDI, Economic Growth, Inflation, and Exchange Rate Volatility

### A Regression Analysis of Iran and Regional Economies

Author: Leila Rezaei  
Research Interests: Applied Economics, International Business, Data Analysis

---

## 📌 Overview

This project investigates the relationship between Foreign Direct Investment (FDI), economic growth, inflation, and exchange-rate volatility in Iran and three regional peer economies: Türkiye, Saudi Arabia, and the United Arab Emirates.

The analysis uses World Bank World Development Indicators (WDI) covering the period 2000–2023.

---

## 🔎 Research Question

Do GDP growth, inflation, and exchange-rate volatility help explain differences in FDI net inflows (% of GDP) across Iran and selected regional economies?

---

## 💡 Hypotheses

- H1: Higher exchange-rate volatility is associated with lower FDI inflows.
- H2: Higher GDP growth is associated with higher FDI inflows.
- H3: Higher inflation is associated with lower FDI inflows.

---

## 📊 Data

Data were obtained from the World Bank World Development Indicators.

| Variable | World Bank Indicator |
|---|---|
| FDI net inflows (% of GDP) | BX.KLT.DINV.WD.GD.ZS |
| GDP growth (annual %) | NY.GDP.MKTP.KD.ZG |
| Inflation (annual %) | FP.CPI.TOTL.ZG |
| Official exchange rate | PA.NUS.FCRF |

### Countries

- Iran
- Türkiye
- Saudi Arabia
- United Arab Emirates

### Period

2000–2023

---

## 🧪 Methodology

The main empirical model uses pooled Ordinary Least Squares (OLS) regression with country fixed effects.

The model specification is:

FDI = β₀ + β₁ GDP Growth + β₂ Inflation + β₃ Exchange Rate Volatility + Country Fixed Effects + ε

Heteroskedasticity-robust HC3 standard errors are used.

### Exchange Rate Volatility

Exchange-rate volatility is measured using the three-year rolling standard deviation of annual percentage changes in the official exchange rate.

---

## 📈 Analysis

The project includes:

- Data cleaning and preparation
- Descriptive statistics
- FDI trends across countries
- Correlation analysis
- Scatter plots
- Fixed-effects regression
- Robust standard errors
- Hypothesis testing
- Robustness analysis using country and year fixed effects
- ## 📌 Regression Results

The regression model explains approximately 48.8% of the variation in FDI net inflows in the sample (R² = 0.488).

Key findings:

- GDP growth: The coefficient is positive (0.0136), but statistically insignificant (p = 0.709).
- Inflation: The coefficient is negative (-0.0180) and statistically significant (p = 0.002), supporting the hypothesis that higher inflation is associated with lower FDI inflows.
- Exchange-rate change: The coefficient is positive (0.0063) and statistically significant (p < 0.001).

Overall, the results provide evidence of a significant negative association between inflation and FDI, while GDP growth does not show a statistically significant relationship with FDI in this sample.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- World Bank API
- Google Colab / Jupyter Notebook

---

## 📁 Repository Structure

`text
fdi-analysis/
│
├── notebooks/
│   ├── fdi_analysis.ipynb
│   ├── README.md
│   └── requirements.txt
│
└── README.md
