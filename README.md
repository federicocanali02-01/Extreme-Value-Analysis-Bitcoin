# Extreme Value Analysis - Bitcoin

A comprehensive statistical analysis of Bitcoin price extremes using Extreme Value Theory (EVT) methods, combining historical Bitcoin data with the Fear and Greed Index to identify and analyze extreme market events.

## 📊 Overview

This project performs an in-depth Extreme Value Analysis on Bitcoin cryptocurrency data from January 1, 2020, to November 30, 2025. The analysis employs two primary statistical methods:

- **Block Maxima (BM)**: Divides the time series into blocks and extracts maximum values
- **Peak Over Threshold (POT)**: Identifies values exceeding a specified threshold

The analysis is enriched with the Fear and Greed Index to provide psychological market context for extreme value events.

## 🎯 Objectives

- Identify extreme price movements in Bitcoin's historical data
- Apply Extreme Value Theory using the `pyextremes` library
- Correlate extreme events with market sentiment through the Fear and Greed Index
- Visualize patterns and distributions of extreme values
- Provide statistical insights into Bitcoin's tail risk behavior

## 📁 Data Sources

### 1. Bitcoin Historical Data
- **Source**: [CoinMarketCap](https://coinmarketcap.com/it/)
- **Period**: January 1, 2020 - November 30, 2025 (historical data)
- **File**: `Bitcoin_historical_data_clean.csv`
- **Features**:
  - `timeOpen`: Market opening time
  - `timeClose`: Market closing time
  - `timeHigh`: Time when daily high was reached
  - `timeLow`: Time when daily low was reached
  - `name`: Cryptocurrency name (Bitcoin)
  - `open`: Opening price
  - `high`: Daily high price
  - `low`: Daily low price
  - `close`: Closing price
  - `volume`: Daily trading volume
  - `marketCap`: Market capitalization
  - `circulatingSupply`: Circulating supply in the market
  - `timestamp`: Data publication timestamp

### 2. Fear and Greed Index
- **Source**: [Alternative.me API](https://alternative.me)
- **File**: `Fear_and_Greed_Index_Bitcoin.csv`
- **Description**: Weighted sentiment index analyzing market psychology based on various factors including volatility, market volume, social media, surveys, Bitcoin dominance, and Google trends
- **Classifications**: Extreme Fear, Fear, Neutral, Greed, Extreme Greed

## 🛠️ Technologies & Libraries

The analysis is implemented in Python using the following libraries:

```python
pandas          # Data manipulation and analysis
numpy           # Numerical computing
matplotlib      # Data visualization
plotly          # Interactive visualizations
seaborn         # Statistical data visualization
pyextremes      # Extreme Value Analysis
sqlalchemy      # Database connectivity (PostgreSQL)
requests        # API calls for Fear and Greed Index
```

## 📋 Requirements

```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
plotly>=5.0.0
seaborn>=0.11.0
pyextremes>=2.0.0
sqlalchemy>=1.4.0
requests>=2.26.0
jupyter>=1.0.0
```

To install the required packages:

```bash
pip install -r requirements.txt
```

## 🚀 Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/federicocanali02-01/Extreme-Value-Analysis-Bitcoin.git
   cd Extreme-Value-Analysis-Bitcoin
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Open the Jupyter Notebook**:
   ```bash
   jupyter notebook Bitcoin.ipynb
   ```

4. **Run the analysis**:
   - Execute cells sequentially to perform the complete analysis
   - Explore visualizations and statistical outputs
   - Modify parameters for custom analysis

## 📈 Analysis Components

### Data Processing
- Data cleaning and transformation
- Feature engineering (day variation, average price)
- Time series formatting
- Database integration with PostgreSQL

### Extreme Value Analysis
- **Block Maxima Method**: Extract maximum values from fixed-time blocks
- **Peak Over Threshold Method**: Identify values exceeding critical thresholds
- Model fitting and parameter estimation
- Return level calculations

### Visualizations
- Price trend analysis
- Distribution of extreme values
- Threshold diagnostics plots
- Fear and Greed Index correlations
- Statistical distribution comparisons

### Market Sentiment Integration
- Merging extreme values with Fear and Greed Index
- Classification distribution analysis
- Correlation between extreme events and market psychology

## 📊 Key Insights

The analysis provides:
- Statistical characterization of Bitcoin price extremes
- Probability estimates for rare events
- Return period calculations for extreme price movements
- Psychological context for extreme market events
- Visual evidence of tail behavior in Bitcoin markets

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📝 License

This project is open source and available for educational and research purposes.

## 👤 Author

**Federico Canali**

- GitHub: [@federicocanali02-01](https://github.com/federicocanali02-01)

## 🙏 Acknowledgments

- Data provided by [CoinMarketCap](https://coinmarketcap.com/)
- Fear and Greed Index from [Alternative.me](https://alternative.me)
- Built with the `pyextremes` library for Extreme Value Analysis