# Financial News Sentiment Analysis and Stock Market Prediction

## Project Overview

This project investigates the relationship between financial news sentiment and stock market movements using Natural Language Processing (NLP), technical analysis, and statistical correlation techniques.

The analysis was conducted as part of a financial analytics challenge focused on understanding how financial news headlines may influence daily stock price behavior. The project combines qualitative financial news data with quantitative historical stock price data to explore whether sentiment extracted from news headlines can help explain or predict stock market trends.

The project follows a complete data analytics workflow including:
- Exploratory Data Analysis (EDA)
- Technical Indicator Analysis
- Sentiment Analysis
- Correlation Analysis
- Data Visualization
- Professional Git/GitHub Workflow

---

# Business Objective

Nova Financial Solutions aims to improve financial forecasting accuracy and operational efficiency through advanced data analytics.

The primary business objective of this project is to:
- Quantify sentiment expressed in financial news headlines
- Analyze historical stock price behavior using technical indicators
- Measure the statistical relationship between news sentiment and stock returns
- Generate actionable insights that may support sentiment-driven investment strategies

---

# Project Tasks

## Task 1 — Exploratory Data Analysis (EDA)

### Objectives
- Explore the structure and quality of the financial news dataset
- Identify patterns in publication frequency and publisher activity
- Analyze textual properties of financial headlines
- Discover common themes and keywords in financial news

### Analysis Performed
- Headline length distribution
- Publisher frequency analysis
- Publication date trend analysis
- Time-series analysis of news volume
- Keyword and topic extraction using NLP techniques
- Publisher domain analysis

### Key Insights
- Certain publishers contributed significantly more articles than others
- Financial news publication volume varied over time with noticeable spikes
- Common themes included earnings reports, price targets, analyst ratings, and FDA approvals

---

## Task 2 — Quantitative Financial Analysis

### Objectives
- Load and prepare historical stock price data
- Compute financial technical indicators
- Visualize market behavior and momentum patterns

### Technical Indicators Computed
- Simple Moving Average (SMA)
- Exponential Moving Average (EMA)
- Relative Strength Index (RSI)
- Moving Average Convergence Divergence (MACD)

### Financial Metrics
- Daily stock returns
- Trend analysis
- Momentum analysis
- Volatility analysis

### Key Insights
- AAPL demonstrated long-term bullish behavior with periods of increased volatility
- Moving averages helped identify trend direction and potential crossover signals
- RSI revealed overbought and oversold market conditions
- MACD highlighted momentum shifts and possible trend reversals

---

## Task 3 — Sentiment and Correlation Analysis

### Objectives
- Perform sentiment analysis on financial news headlines
- Align news publication dates with stock trading dates
- Measure the relationship between sentiment and stock returns

### Sentiment Analysis
The VADER sentiment analysis model from NLTK was used to compute sentiment scores for financial news headlines.

VADER was selected because:
- It performs well on short text content such as headlines
- It is computationally efficient
- It produces normalized sentiment scores between -1 and +1

### Correlation Analysis
The project computed:
- Average daily sentiment scores
- Daily stock returns
- Pearson correlation coefficients between sentiment and returns

### Visualizations
- Scatter plot of sentiment vs daily returns
- Bar chart of average returns by sentiment category

### Key Findings
- Financial news sentiment showed a weak-to-moderate relationship with stock returns
- Positive sentiment generally aligned with stronger market performance
- Market behavior is influenced by many additional external factors beyond news sentiment alone

---

# Datasets Used

## Financial News Dataset

The Financial News and Stock Price Integration Dataset (FNSPID) contains:
- Financial news headlines
- Publishers
- Publication timestamps
- Stock ticker symbols
- Article URLs

### Main Fields
- `headline`
- `publisher`
- `date`
- `stock`
- `url`

---

## Historical Stock Price Dataset

Historical stock price data was obtained using the YFinance Python library.

### Main Fields
- `Date`
- `Open`
- `High`
- `Low`
- `Close`
- `Adj Close`
- `Volume`

---

# Technologies and Libraries Used

## Programming Language
- Python

## Data Analysis
- Pandas
- NumPy

## Data Visualization
- Matplotlib
- Seaborn

## NLP and Sentiment Analysis
- NLTK
- VADER Sentiment Analyzer

## Technical Analysis
- TA-Lib
- PyNance

## Statistical Analysis
- SciPy

## Development Tools
- Git
- GitHub
- GitHub Actions
- Jupyter Notebook

---

# Project Structure

```text
financial-news-project/
│
├── .github/
│   └── workflows/
│       └── unittests.yml
│
├── notebooks/
│   ├── 1_financial_news_eda.ipynb
│   ├── 2_technical_analysis.ipynb
│   └── 3_sentiment_correlation.ipynb
│
├── data/
│
├── .gitignore
├── requirements.txt
└── README.md