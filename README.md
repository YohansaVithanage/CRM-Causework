# Market Analysis and Stock Segmentation Using RFM

## Project Overview
This project analyses S&P 500 companies using Business Intelligence techniques to identify stock groups based on historical risk, return and trading activity.

Two feature groups are analysed:
- Risk/Return: Mean Weekly Return and Beta.
- RFM: Recency, Frequency and Monetary.

Ward's Hierarchical Clustering and K-means are used to identify and compare stock segments.

## Dataset
- Data source: Yahoo Finance and Wikipedia.
- Benchmark: S&P 500 Index (^GSPC).
- Study period: 1 January 2021 – 1 January 2025.
- Data frequency: Daily stock prices and trading volumes.

## Technologies Used
- Python and Google Colab
- pandas and NumPy
- yfinance
- SciPy
- scikit-learn
- Matplotlib

## Methodology
**Task 1:** Data collection, validation, weekly return, beta and adapted RFM calculations.

**Task 2:** Feature preparation, Ward clustering, K-means clustering, cluster comparison and sensitivity analysis.

**Task 3:** Data mart design, business interpretation and critical review.

## Repository Contents
- `CRM_Coursework.ipynb` – Main Python notebook.
- `weekly_features.csv` – Weekly return and beta results.
- `rfm_features.csv` – RFM results.
- `final_feature_table_with_clusters.csv` – Feature values and cluster assignments.
- `inclusion_exclusion_log.csv` – Inclusion and exclusion records.
- `daily_data_quality_report.csv` – Data quality results.
- `corporate_action_audit.csv` – Corporate action audit.
- `corporate_action_flags.csv` – Corporate action flags.
- `run_metadata.json` – Run information and package versions.

## How to Run
1. Open the notebook using Google Colab.
2. Run all cells from beginning to end.
3. Install the required libraries if prompted.
4. Allow the notebook to retrieve the historical market data.
5. Review the generated results and visualisations.

## Limitations
- The current S&P 500 constituent list is applied retrospectively, creating potential survivorship bias.
- Historical clusters do not predict future stock performance.
- Monetary represents approximate traded value, not market capitalisation.
