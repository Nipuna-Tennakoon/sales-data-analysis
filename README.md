# Sales Demand Prediction Project

This project focuses on analyzing sales data to understand patterns in product demand and price variations. The insights gained are used to prepare data for predictive modeling.

## Project Overview

The project is divided into two main phases:
1. **Exploratory Data Analysis (EDA)**
2. **Time Series Analysis (TS Analysis)**

---

## 1. Exploratory Data Analysis (EDA)

The EDA phase involves analyzing the sales dataset to uncover patterns and trends. Below are the key steps and findings:

### Steps:
- Imported the dataset and necessary libraries for data manipulation and visualization.
- Conducted descriptive analysis on the sales dataset.
- Focused on the first five high-demand products for detailed analysis.
- Visualized the price and quantity sold for these products over time.

### Key Findings:
- High-priced products have low sales volume.
- The demand for products is highest on **Monday** and **Tuesday**, while **Sunday** has the lowest demand.
- Temporal patterns were observed in both price and demand.

### Outputs:
- Visualizations of price and quantity trends for the top five products.
- Dataframes saved for prediction purposes.

---

## 2. Time Series Analysis (TS Analysis)

The TS Analysis phase focuses on preparing the data for predictive modeling by analyzing stationarity and autocorrelation.

### Steps:
- Conducted stationarity tests on selling prices and demand for the top five products.
- Observed that:
  - Product A's price series is non-stationary.
  - Demand for all five products is non-stationary.
- Generated ACF and PACF plots for further analysis.
- Transformed non-stationary series into stationary series for modeling.

### Outputs:
- Pivot tables saved for training purposes.

---

## Files in the Repository

- **`eda-visualization.ipynb`**: Notebook for exploratory data analysis and visualizations.
- **`ts-analysis.ipynb`**: Notebook for time series analysis and preparation for predictive modeling.
- **`summary.txt`**: Document summarizing the project lifecycle and decisions made.

---

## Future Work

- Transform non-stationary series into stationary for all products.
- Build predictive models for sales demand forecasting.
- Explore additional features to improve model accuracy.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone <repository-url>
