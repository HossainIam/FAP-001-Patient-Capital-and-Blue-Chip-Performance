# An Institutional Analysis of the German Corporate Ecosystem and the DAX-5 tyhis 

## Project Architecture

```text
FAP-001-Patient-Capital-German-Equity/
│
├── README.md                # Executive Summary, Abstract, and Quick-Start Guide
├── requirements.txt         # Package dependencies (pandas, numpy, yfinance, matplotlib)
├── config/
│   └── settings.yaml        # Tickers (SAP, SIE, ALV, DTE, MBG) and macro indicators
│
├── data/
│   ├── raw/                 # Stock price history and ECB interest rate data
│   └── processed/           # Extracted fundamental metrics (Margins, Backlogs, Debt-to-Equity)
│
├── docs/                    # Structural research papers (Hausbank & Comparative Frameworks)
│   ├── 01_abstract_intro.md 
│   ├── 02_comparative.md    
│   └── final_paper.pdf      
│
├── notebooks/               # Exploratory Data Analysis
│   ├── macro_analysis.ipynb 
│   └── equity_analysis.ipynb
│
└── src/                     # Production Python scripts
    ├── data_loader.py       # Pulls yfinance data and macroeconomic metrics
    ├── fundamental_engine.py# Calculates Return on Invested Capital (ROIC), FCF Yield, Margins
    └── valuation_engine.py  # Builds the Patient-Capital Discounted Cash Flow (DCF) model
\_ _ _
