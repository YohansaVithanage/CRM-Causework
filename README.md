# Market Analysis and Stock Segmentation Using RFM

## 1. Project Overview

This project analyses S&P 500 companies using Business Intelligence techniques to identify stock groups based on their historical risk, return and trading activity.

Two feature groups are used:
- **Risk/Return:** Mean Weekly Return and Beta.
- **Trading Activity (RFM):** Recency, Frequency and Monetary.

The project applies Ward's Hierarchical Clustering and K-means clustering to identify and compare stock segments.

## 2. Dataset and Data Sources

- **Stock constituents:** S&P 500 companies from Wikipedia.
- **Historical market data:** Yahoo Finance using the yfinance Python library.
- **Benchmark:** S&P 500 Index (^GSPC).
- **Study period:** 1 January 2021 – 1 January 2025 (end date exclusive).
- **Data frequency:** Daily stock prices and trading volumes.

## 3. Technologies Used

- Python
- Google Colab
- pandas
- NumPy
- yfinance
- SciPy
- scikit-learn
- Matplotlib
- requests
- lxml

## 4. Project Methodology

### Task 1 – Data Preparation and Feature Engineering
- S&P 500 ticker selection and historical data collection.
- Data validation and quality checks.
- Weekly return and beta calculations.
- Adapted RFM feature calculation.

### Task 2 – Stock Segmentation and Sensitivity Analysis
- Feature preparation and standardisation.
- Ward's Hierarchical Clustering.
- K-means clustering.
- Cluster profile comparison.
- RFM correlation analysis.
- Monetary removal sensitivity analysis.

### Task 3 – Business Intelligence and Critical Review
- Data mart design.
- Business interpretation of stock segments.
- Evaluation of findings and analytical limitations.

## 5. Repository Files

The repository includes:

- `CRM_Coursework.ipynb` – Main Python analysis notebook.
- `sp500_constituents.csv` – S&P 500 constituent data.
- `weekly_features.csv` – Weekly return and beta results.
- `rfm_features.csv` – RFM feature results.
- `final_feature_table_with_clusters.csv` – Feature values and cluster assignments.
- `inclusion_exclusion_log.csv` – Inclusion and exclusion records.
- `daily_data_quality_report.csv` – Data quality results.
- `corporate_action_audit.csv` – Corporate action audit.
- `corporate_action_flags.csv` – Corporate action flags.
- `run_metadata.json` – Run information and package versions.

## 6. How to Run the Project

1. Open Google Colab.
2. Upload or open the `.ipynb` notebook.
3. Run all cells from beginning to end.
4. Install the required libraries if prompted.
5. Allow the notebook to retrieve the historical market data.
6. Review the generated tables, charts and clustering results.

An internet connection is required for downloading the market data.

## 7. Limitations

- The current S&P 500 constituent list is applied to historical data, creating potential survivorship bias.
- Historical clusters do not predict future stock performance.
- Beta represents historical market sensitivity.
- Monetary is an approximate traded-value measure, not market capitalisation or investment inflow.

## 8. References

- Wikipedia – List of S&P 500 Companies.
- Yahoo Finance – Historical Market Data.
- Scikit-learn – Clustering Documentation.
- Ward (1963) – Hierarchical Grouping to Optimize an Objective Function.
- MacQueen (1967) – Some Methods for Classification and Analysis of Multivariate Observations.
