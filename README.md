# Supply Chain Analytics Project

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-green.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

<p align="center">
  <img src="images/Screenshot (210).png" alt="Screenshot Preview" width="90%"/>
</p>

A comprehensive Supply Chain Analytics project demonstrating end-to-end data analysis capabilities including data collection, cleaning, exploratory data analysis, KPI calculation, visualization, and predictive analytics.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Key Insights](#key-insights)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## 🎯 Project Overview

This project analyzes supply chain performance using both real-world data from the **World Bank Open Data** and synthetic operational data. The analysis covers:

- **Global Logistics Performance** comparison across countries
- **Order Fulfillment Analysis** with 5,000+ transactions
- **Supplier Performance Evaluation** across 20 suppliers
- **Shipping & Logistics Optimization** insights
- **Demand Forecasting** using machine learning
- **Interactive Dashboards** for real-time monitoring

### Key Performance Indicators Tracked:

| KPI | Description | Target |
|-----|-------------|--------|
| Order Fulfillment Rate | % of orders successfully delivered | >95% |
| On-Time Delivery Rate | % of orders delivered on time | >90% |
| Perfect Order Rate | % of orders delivered without issues | >85% |
| Lead Time | Average time from order to delivery | <20 days |
| Delay Rate | % of orders with delays | <10% |

---

## 📊 Data Sources

### 1. World Bank Open Data (Real-world)
- **Source**: [World Bank Open Data](https://data.worldbank.org/)
- **Countries**: USA, China, Germany, Japan, UK, France, India, Korea, Brazil, Mexico
- **Indicators**:
  - Logistics Performance Index (Track & Trace, Service Quality, Customs)
  - Trade Statistics (Exports, Imports, Trade % of GDP)
  - Lead Times (Export/Import duration)
  - Shipping Connectivity Index
- **Time Period**: 2017-2024

### 2. Synthetic Supply Chain Operations Data
- **Orders**: 5,000 transaction records (2022-2023)
- **Products**: 50 products across 6 categories
- **Suppliers**: 20 suppliers from 7 countries
- **Warehouses**: 8 warehouses across 5 regions
- **Customers**: 300 customers in different segments

---

## 📁 Project Structure

```
supply_chain_analytics/
│
├── 📓 Supply_Chain_Analytics.ipynb    # Main Jupyter Notebook with all analysis
├── 📄 README.md                        # Project documentation
├── 📄 requirements.txt                 # Python dependencies
│
├── 📂 data/                           # Data files
│   ├── world_bank_logistics_data.csv  # World Bank data
│   ├── orders.csv                     # Order transactions
│   ├── products.csv                   # Product master data
│   ├── suppliers.csv                  # Supplier master data
│   ├── warehouses.csv                 # Warehouse master data
│   ├── customers.csv                  # Customer master data
│   └── kpi_summary_report.csv         # Generated KPI report
│
├── 📂 images/                         # Static visualizations
│   ├── logistics_performance_comparison.png
│   ├── trade_statistics.png
│   ├── order_trends.png
│   ├── order_distributions.png
│   ├── shipping_analysis.png
│   ├── kpi_dashboard.png
│   ├── supplier_performance.png
│   ├── demand_forecast.png
│   └── correlation_matrix.png
│
└── 📂 dashboards/                     # Interactive HTML dashboards
    ├── interactive_dashboard.html
    ├── category_sunburst.html
    └── geographic_analysis.html
```

---

## ✨ Key Features

### 1. Data Collection & Integration
- Automated data retrieval from World Bank API
- Synthetic data generation for operational metrics
- Data merging and relationship mapping

### 2. Data Cleaning & Preprocessing
- Missing value handling
- Outlier detection using IQR method
- Feature engineering (derived metrics)
- Data type conversions

### 3. Exploratory Data Analysis (EDA)
- Time series analysis of order trends
- Category-wise performance comparison
- Shipping mode efficiency analysis
- Geographic distribution analysis

### 4. Supply Chain KPIs
- Order Fulfillment Rate
- On-Time Delivery Rate
- Perfect Order Rate
- Lead Time Analysis
- Inventory Turnover Ratio
- Cost Analysis (Shipping, Total Cost)

### 5. Advanced Analytics
- **Supplier Performance Scoring**: Reliability vs. Performance correlation
- **Demand Forecasting**: Linear regression model for demand prediction
- **Correlation Analysis**: Relationship between key variables
- **Delay Pattern Analysis**: Root cause identification

### 6. Visualizations & Dashboards
- **Static Charts**: Matplotlib & Seaborn visualizations
- **Interactive Dashboards**: Plotly-based HTML dashboards
- **Geographic Maps**: Country-wise performance visualization
- **Sunburst Charts**: Hierarchical category analysis

---

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- Anaconda (recommended) or pip
- Jupyter Notebook

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/supply_chain_analytics.git
cd supply_chain_analytics
```

### Step 2: Create Virtual Environment (Recommended)
```bash
# Using conda
conda create -n supply_chain python=3.8
conda activate supply_chain

# Using venv
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook
```bash
jupyter notebook Supply_Chain_Analytics.ipynb
```

---

## 📖 Usage

### Running the Analysis

1. **Open the Notebook**:
   ```bash
   jupyter notebook Supply_Chain_Analytics.ipynb
   ```

2. **Run All Cells**:
   - Use `Cell` → `Run All` from the menu
   - Or press `Shift + Enter` to run cells sequentially

3. **Explore Results**:
   - View generated visualizations in the `images/` folder
   - Open interactive dashboards in the `dashboards/` folder
   - Check the KPI summary report in `data/kpi_summary_report.csv`

### Customizing the Analysis

To analyze your own supply chain data:

1. Replace CSV files in the `data/` folder with your data
2. Update column mappings in the notebook if needed
3. Adjust KPI thresholds based on your business requirements
4. Re-run the notebook to generate updated insights

---

## 🔍 Key Insights

### Overall Performance
- **Total Orders Processed**: 5,000
- **Total Revenue**: $62.5 Million
- **Average Order Value**: $12,500
- **Order Fulfillment Rate**: 81.3%
- **On-Time Delivery Rate**: 78.5%

### Shipping & Logistics
- **Best Performing Mode**: Air (highest on-time rate)
- **Most Cost-Effective Mode**: Sea (lowest cost per unit)
- **Average Lead Time**: 21.3 days
- **Shipping Cost Ratio**: 4.2% of revenue

### Supplier Performance
- **Top Supplier**: 95%+ on-time delivery rate
- **Underperforming Suppliers**: 60-70% on-time rate
- **Best Country**: Germany (highest reliability score)
- **Recommendation**: Review contracts with bottom 20% performers

### Areas for Improvement
1. **Delay Rate**: 15.2% (Target: <10%)
2. **Cancellation Rate**: 4.4% (Target: <3%)
3. **Low Stock Issues**: 12% of orders affected

### Recommendations
1. Implement supplier scorecards for continuous monitoring
2. Optimize shipping mode selection based on cost-time tradeoffs
3. Review reorder points to reduce stockouts
4. Deploy predictive analytics for demand forecasting
5. Integrate real-time shipment tracking

---

## 📈 Visualizations

### Static Visualizations
All static charts are saved in the `images/` folder:

| Visualization | Description |
|---------------|-------------|
| Logistics Performance Comparison | Country-wise LPI scores |
| Trade Statistics | Exports vs Imports analysis |
| Order Trends | Monthly volume and revenue trends |
| Shipping Analysis | Cost, lead time, and performance by mode |
| KPI Dashboard | Comprehensive performance metrics |
| Supplier Performance | Supplier ranking and analysis |
| Demand Forecast | Predicted vs actual demand |
| Correlation Matrix | Variable relationships |

### Interactive Dashboards
Open HTML files in your browser:

1. **interactive_dashboard.html**: Main performance dashboard with time-series charts
2. **category_sunburst.html**: Hierarchical revenue breakdown
3. **geographic_analysis.html**: World map with supplier performance

---

## 🛠️ Technologies Used

### Data Manipulation
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing

### Visualization
- **Matplotlib**: Static visualizations
- **Seaborn**: Statistical visualizations
- **Plotly**: Interactive charts and dashboards

### Machine Learning
- **Scikit-learn**: Demand forecasting model

### Data Source
- **World Bank Open Data API**: Real-world logistics data

---

## 🔮 Future Enhancements

- [ ] **Real-time Data Integration**: Connect to live ERP systems
- [ ] **Advanced Forecasting**: Implement ARIMA, Prophet, or LSTM models
- [ ] **Inventory Optimization**: EOQ and safety stock calculations
- [ ] **Network Optimization**: Warehouse location analysis
- [ ] **Risk Analysis**: Supply chain risk scoring
- [ ] **What-if Analysis**: Scenario modeling tool
- [ ] **Automated Reporting**: Email reports with scheduled execution

---

## 👨‍💻 Author

ANthony Michael
- LinkedIn: [My LinkedIn Profile](https://linkedin.com/in/anthony-michael-b36382259)
- GitHub: [My GitHub Profile](https://github.com/anthonymike180)
- Email: anthonymike9110@gmail.com

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **World Bank Open Data** for providing free access to global development data
- **Open-source community** for the amazing Python libraries
- **Supply Chain Management** professionals for domain knowledge

---

**⭐ Star this repository if you find it helpful!**
