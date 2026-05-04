# Cloud-Cost-Intelligence-Dashboard

A data analytics project exploring cloud cost management principles through simulated AWS billing data analysis.

## Overview

This project demonstrates end-to-end data pipeline development and cost analysis techniques used in cloud financial operations. It processes billing data, detects anomalies, forecasts trends, and provides optimization insights.

## Features

- **Data Generation** - Simulates realistic AWS billing records
- **ETL Pipeline** - Cleans, transforms, and organizes billing data
- **Anomaly Detection** - Identifies unusual spending patterns
- **Cost Forecasting** - Predicts future cloud spending trends
- **Optimization Analysis** - Recommends Reserved Instance strategies
- **Interactive Dashboard** - Visualizes insights with charts and metrics

## Tech Stack

- **Python 3.10+**
- **Pandas** - Data manipulation & analysis
- **NumPy** - Numerical computing
- **Streamlit** - Interactive dashboard
- **Plotly** - Data visualization
- **Faker** - Sample data generation

## Installation

1. **Clone or download this project**

2. **Install Python 3.10+** from [python.org](https://www.python.org)
   - During installation, check "Add Python to PATH"

3. **Install dependencies**
   ```bash
   python -m pip install -r requirements.txt
   ```

## Usage

### Run Complete Analysis Pipeline
```bash
python run_all.py
```

This generates sample data and runs all analysis modules. Output files:
- `anomaly_report.csv` - Detected cost anomalies
- `forecast_report.csv` - Cost predictions
- `ri_optimizer_report.csv` - Reserved Instance recommendations

### Launch Interactive Dashboard
```bash
python -m streamlit run dashboard.py
```

Opens browser at `http://localhost:8501` with visualizations and insights.

### Run Individual Modules
```bash
python generate_data.py          # Generate sample billing data
python etl_pipeline.py           # Process & clean data
python anomaly_detector.py       # Detect spending anomalies
python forecaster.py             # Predict future costs
python ri_optimizer.py           # Optimize Reserved Instances
```

## Project Structure

```
ccloud/
├── README.md
├── requirements.txt
├── run_all.py                  # Main pipeline orchestrator
├── generate_data.py            # Simulates AWS billing data
├── etl_pipeline.py             # Data cleaning & transformation
├── anomaly_detector.py         # Anomaly detection algorithm
├── forecaster.py               # Cost forecasting model
├── ri_optimizer.py             # Reserved Instance recommendations
├── dashboard.py                # Streamlit dashboard
├── anomaly_report.csv          # Generated anomaly findings
├── forecast_report.csv         # Generated forecasts
└── ri_optimizer_report.csv     # Generated RI recommendations
```

## Key Learnings

This project explores:
- Cloud cost management principles
- ETL pipeline design patterns
- Time-series forecasting techniques
- Anomaly detection algorithms
- Data visualization best practices
- Cost optimization strategies

## How to Stop

Press **Ctrl + C** in the terminal to stop any running process.

## Troubleshooting

**Python not found:**
```bash
python -m pip install -r requirements.txt
python -m streamlit run dashboard.py
```

**Streamlit not recognized:**
Use `python -m streamlit` instead of just `streamlit`

## Future Enhancements

- [ ] Connect to real AWS Billing API
- [ ] Add multi-cloud cost analysis (Azure, GCP)
- [ ] Implement advanced ML forecasting models
- [ ] Add cost allocation by department/project
- [ ] Export reports to PDF format

## License

Personal learning project

---

**Built while exploring cloud cost management concepts**
