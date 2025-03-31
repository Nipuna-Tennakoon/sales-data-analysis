# Sales Demand & Product Price Prediction Project

This project focuses on analyzing sales data to understand patterns in product demand and price variations. The insights gained are used to prepare data for predictive modeling.

## Project Overview

The project is divided into three main phases:
1. **Exploratory Data Analysis (EDA)**
2. **Time Series Analysis (TS Analysis)**
3. **Training and Model Development**

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

## 3. Training and Model Development

The training phase focuses on building predictive models for sales demand forecasting.

### Steps:
- Set the objectives for the modeling phase.
- Used the price dataset for modeling after transforming it into a stationary series.
- Developed an ARIMA model for forecasting.
- Tuned the model to obtain the optimal `forecasting_length` and ARIMA parameters (`p`, `d`, `q`).

### Outputs:
- Optimal ARIMA parameters and forecasting length identified for accurate predictions.

---

## Files in the Repository

- **`eda-visualization.ipynb`**: Notebook for exploratory data analysis and visualizations.
- **`ts-analysis.ipynb`**: Notebook for time series analysis and preparation for predictive modeling.
- **`training.ipynb`**: Notebook for training and model development.
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
   ```
2. Open the notebooks (`eda-visualization.ipynb`, `ts-analysis.ipynb`, and `training.ipynb`) in Jupyter Notebook or VS Code.
3. Follow the steps in each notebook to reproduce the analysis and modeling.

---

## License

This project is for educational purposes. Please contact the author for permissions regarding commercial use.
