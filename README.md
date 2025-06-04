# Data Integration and Automation Project

This project demonstrates how to automate a data pipeline that merges weekly synthetic sales data with real-world economic indicators using the FRED API. It also includes integrity checks and alerts for anomalies or data quality issues.

## 📌 Overview

This solution was built to simulate a real-world data integration scenario where business data (like sales) needs to be combined with economic indicators (like gas prices and CPI) for better analysis.

## 🚀 Features

- Generates synthetic weekly sales data
- Fetches real economic indicators via FRED API
- Merges and aligns data by week
- Checks for missing values and anomalies
- Logs or sends alerts if data issues are found
- Final merged dataset is saved to CSV

## 📂 Files Included

- `Data Integration and Automation.ipynb`: Main notebook containing the entire project
- `merged_sales_data.csv`: Final output after merging and validation
- `Documentation.txt`: Brief explanation of approach, assumptions, and instructions

## ⚙️ Execution Instructions

1. Clone or download this repository.
2. Open the `Data Integration and Automation.ipynb` file in Jupyter Notebook or VS Code.
3. Replace the `api_key` in `fetch_economic_data()` with your own FRED API key.
4. Run all cells sequentially to generate and merge the data.
5. The final merged data will be saved to `merged_sales_data.csv`.

## 📌 Assumptions

- FRED API key is valid and has access to required economic indicators.
- Synthetic data is assumed to represent sales for 2023–2024 weekly.
- SMTP server is configured only if email alerts are required.

## 🧪 Data Validation Logic

- Checks for missing critical sales values (`Units Sold`, `Price`, `Discount`, `Revenue`)
- Detects outliers in `Units Sold` using Z-score method
- Ensures economic data is not missing after merge

## 📝 Author

Amit Dubey  
Email: amitdubeypa@gmail.com

## 🧾 License

This project is for learning and demonstration purposes only.

