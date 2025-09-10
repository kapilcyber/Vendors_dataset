# Vendor Transaction Analysis (EDA)

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** on a vendor transactions dataset (monthly CSVs) to identify patterns and factors affecting customer purchasing behavior and product sales.

Vendor transaction analysis is critical for businesses to uncover key sales drivers, best-selling products, seasonal trends, and geographic sales performance. This project merges transactional records across months to provide actionable insights.

## 📂 Dataset

- **Files:** Monthly transaction CSVs (merged to `all_data_copy.csv`)
- **Rows:** ~tens of thousands of orders  
- **Key Variables:**  
  - `Order ID`  
  - `Product`  
  - `Quantity Ordered`  
  - `Price Each`  
  - `Order Date`  
  - `Purchase Address`  
  - `Month` (derived)  
  - `City` (derived)  
  - `Sales` (computed as `Quantity Ordered * Price Each`)

## ⚙️ Steps Performed

### Data Loading

- Reads all monthly transaction CSV files using `pandas`.
- Merges individual files into one comprehensive dataset.
- Checks shape, missing data, and basic info.

### Data Preprocessing

- Extracts features such as `Month`, `City`, and computes `Sales` for each transaction.
- Handles missing and duplicate values.
- Formats date and address fields for analysis.

### Exploratory Data Analysis (EDA)

- Analyzes sales trends by month, city, and product.
- Identifies top-selling products and high-revenue regions.
- Explores peak hours and order timing patterns.
- Generates summary metrics and aggregated tables.

### Insights

- Reveals busiest sales months and high-performing cities.
- Identifies products contributing most to revenue.
- Uncovers time slots when orders peak.
- Provides vendor-centric guidelines for inventory and marketing.

## 📊 Visualizations

- **Monthly and city-wise sales bar plots**
- **Product-wise sales distributions**
- **Revenue time series**
- **Order count heatmaps**
- **Top product charts**

## 🛠️ Tech Stack

- Python
- pandas, numpy
- matplotlib, seaborn

## 🚀 How to Run

1. Clone this repository:

git clone https://github.com/yourusername/vendor-transaction-analysis.git

2. Place all monthly transaction CSV files in the `Sales_Data` directory.
3. Open and run `SalesAnalysis.ipynb` in Jupyter Notebook or Google Colab.
