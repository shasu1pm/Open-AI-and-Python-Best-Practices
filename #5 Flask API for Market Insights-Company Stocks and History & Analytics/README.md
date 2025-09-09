# Stock Market Analysis API Suite

> As a Product Manager from a non-coding background, I built this project with 20% traditional coding and 80% pure 'Vibe Coding' — blending intuition, design sense, and problem-solving energy into the flow.

## 🚀 Project Overview

This comprehensive Stock Market Analysis API Suite provides four powerful endpoints for financial data analysis and insights. Built using Flask and Yahoo Finance API, this project offers real-time and historical market data with advanced analytical capabilities.

## 📊 Core Features

### 1. Company Information Endpoint
- **Purpose**: Retrieve detailed company information and corporate data
- **Key Features**:
  - Company name, business summary, industry, and sector information
  - Key officers' names and titles
  - Input validation for stock symbols
  - Comprehensive error handling and JSON responses
  - Support for both company names and stock symbols

### 2. Stock Market Data Endpoint
- **Purpose**: Fetch real-time stock market data with comprehensive metrics
- **Key Features**:
  - Current market price and trading status
  - Daily performance metrics (open, high, low, close)
  - Price changes and percentage movements
  - 52-week range analysis
  - Trading volume and market capitalization
  - Real-time quote timestamps

### 3. Historical Market Data Endpoint
- **Purpose**: Access historical market data with flexible time ranges
- **Key Features**:
  - Customizable date ranges (DD/MM/YYYY format)
  - Multiple interval options (1d, 1wk, 1mo, 5d)
  - OHLC (Open, High, Low, Close) price data
  - Volume analysis
  - Dividend and stock split information
  - Comprehensive data validation

### 4. Analytical Insights Endpoint
- **Purpose**: Advanced financial analysis and visualization system
- **Key Features**:
  - Technical indicators (RSI, MACD, Bollinger Bands)
  - Moving averages (SMA, EMA)
  - Risk metrics (Volatility, Sharpe Ratio, Beta)
  - Drawdown analysis and anomaly detection
  - Interactive visualizations with Plotly
  - Comprehensive performance reports

## 🛠️ Technology Stack

- **Backend**: Flask (Python web framework)
- **Data Source**: Yahoo Finance API (yfinance)
- **Data Processing**: Pandas, NumPy
- **Visualization**: Plotly, Matplotlib, Seaborn
- **Development Environment**: Jupyter Notebooks

## 📋 API Endpoints

### Company Information
```
GET /api/company/<symbol>
POST /api/company/name
```

### Stock Market Data
```
POST /api/stock/market-data
GET /api/stock/market-data/<symbol>
```

### Historical Data
```
POST /historical-data
```

### Analytical Insights
```
Interactive analysis with comprehensive reporting
```

## 🔧 Installation & Setup

1. **Clone the repository**
```bash
git clone <repository-url>
cd stock-market-api-suite
```

2. **Install dependencies**
```bash
pip install flask yfinance pandas numpy matplotlib plotly seaborn requests
```

3. **Run the application**
```bash
python app.py
```

## 📖 Usage Examples

### Company Information Lookup
```json
POST /api/company/name
{
  "company_name": "Apple Inc"
}
```

### Real-time Market Data
```json
POST /api/stock/market-data
{
  "company_name": "Microsoft"
}
```

### Historical Data Request
```json
POST /historical-data
{
  "company_name": "Google",
  "start_date": "01/01/2023",
  "end_date": "31/12/2023",
  "interval": "1d"
}
```

## 🎯 Key Capabilities

### Data Validation & Error Handling
- Comprehensive input validation
- Graceful error handling with informative messages
- Symbol resolution from company names
- Date format validation

### Financial Metrics
- **Performance**: Total returns, cumulative returns
- **Risk**: Volatility, Sharpe ratio, maximum drawdown
- **Technical**: RSI, MACD, Bollinger Bands, moving averages
- **Comparative**: Beta analysis vs benchmarks

### Interactive Features
- User-friendly input interfaces
- Real-time data fetching
- Interactive visualizations
- Comprehensive reporting

## 📊 Supported Companies

The system includes mappings for major companies including:
- **Tech Giants**: Apple, Microsoft, Google/Alphabet, Amazon, Meta
- **Growth Stocks**: Tesla, Netflix, NVIDIA, Zoom, Spotify
- **Enterprise**: IBM, Oracle, Salesforce, Adobe, Intel
- **Financial**: Visa, Mastercard, PayPal
- **Consumer**: Disney, McDonald's, Nike, Starbucks, Walmart

## 🔍 Data Sources & Accuracy

- **Primary Source**: Yahoo Finance API
- **Real-time Data**: Live market prices and trading information
- **Historical Coverage**: Extensive historical data availability
- **Update Frequency**: Real-time for current data, daily for historical

## 🚀 Future Enhancements

- Portfolio analysis capabilities
- Machine learning predictions
- Advanced charting features
- Real-time alerts and notifications
- Database integration for data persistence
- RESTful API documentation with Swagger

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.


*Built with passion for financial data analysis and market insights* 📈