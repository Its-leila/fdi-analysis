# FDI, Economic Growth, and Inflation: A Regression Analysis

## Abstract
This project examines whether GDP growth, inflation, and exchange rate volatility
significantly affect Foreign Direct Investment (FDI) net inflows in Iran, compared
to regional peer economies (Turkey, Saudi Arabia, UAE). Using World Bank data
(2000–2023), a pooled OLS regression with country fixed effects is estimated to
test three hypotheses about the drivers of FDI.

## Research Question
Do GDP growth, inflation, and exchange rate volatility significantly affect FDI
net inflows (% of GDP) in Iran and regional economies?

## Hypotheses
- H1: Higher exchange rate volatility is associated with lower FDI inflows.
- H2: Higher GDP growth is associated with higher FDI inflows.
- H3: Higher inflation is associated with lower FDI inflows.

## Data Source
World Bank World Development Indicators (WDI), accessed via the wbdata Python
package:
- BX.KLT.DINV.WD.GD.ZS — FDI, net inflows (% of GDP)
- NY.GDP.MKTP.KD.ZG — GDP growth (annual %)
- FP.CPI.TOTL.ZG — Inflation, consumer prices (annual %)
- PA.NUS.FCRF — Official exchange rate (LCU per US$, period average)

Countries: Iran, Turkey, Saudi Arabia, United Arab Emirates. Period: 2000–2023.

## Methodology
Pooled OLS regression with country fixed effects and heteroskedasticity-robust
standard errors (HC3), estimated with statsmodels.

## How to Run
The easiest way — no installation required:

1. Open notebooks/fdi_analysis.ipynb in Google Colab (colab.research.google.com).
2. Run all cells from top to bottom (Runtime → Run all).
3. The notebook fetches live data from the World Bank API, cleans it, runs
   exploratory analysis, and estimates the regression model.

To run locally instead:
pip install -r requirements.txt
jupyter notebook notebooks/fdi_analysis.ipynb

## Repository Structure
fdi-analysis/
├── data/                       # cleaned dataset saved after running the notebook
├── notebooks/
│   └── fdi_analysis.ipynb      # full analysis: EDA, regression, interpretation
├── README.md
└── requirements.txt

## Key Findings
(To be filled in after running the notebook — see Section 6 of the notebook for
the interpretation template.)

## Limitations
- Small sample size (4 countries × ~20 years) limits statistical power.
- FDI is influenced by many unobserved factors (sanctions, geopolitical events,
  oil prices) not captured in this model.
- World Bank data for Iran has gaps in some years due to reporting limitations.
- Regression results here indicate association, not causation.

## Author
Leila Rezaei — Bachelor of Business Administration, Islamic Azad University
Research interests: Applied economics, financial management, international business
