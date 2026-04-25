# Lending Club Loan Default Prediction Analysis

This repository contains a comprehensive analysis of Lending Club loan data, focusing on building a predictive model for loan default and preparing data for interactive visualization in Tableau.

## Project Overview

The goal of this project is to:
1.  **Clean and preprocess** a large dataset of historical Lending Club loan applications.
2.  **Perform Exploratory Data Analysis (EDA)** to understand trends, distributions, and relationships related to loan default.
3.  **Conduct statistical analysis** to identify key factors influencing default risk.
4.  **Develop a preliminary predictive model** using Logistic Regression.
5.  **Prepare aggregated datasets** for interactive dashboards in Tableau.

## Dataset

The primary dataset used is the Lending Club Loan Status data from 2007-2020Q3 (`Loan_status_2007-2020Q3.gzip`). It contains detailed information about loan applicants, loan characteristics, and repayment status.

## Folder Structure

*   `data/raw/`: Contains the original raw dataset.
*   `data/processed/`: Stores cleaned, preprocessed, and aggregated datasets.
*   `notebooks/`: Contains the Jupyter/Colab notebooks documenting the analysis steps.
*   `tableau/screenshots/`: Stores screenshots of key visualizations from EDA and potentially Tableau dashboards.
*   `tableau/dashboard_links.md`: A markdown file to link to published Tableau dashboards.
*   `docs/`: Contains supplementary documentation, such as the data dictionary.

## Analysis Highlights

-   **Data Cleaning:** Handled missing values, converted data types, and capped outliers.
-   **Feature Engineering:** Derived new features like `credit_age_months`, `fico_avg`, and `loan_to_income`.
-   **EDA:** Visualized default rates by year, grade, state, loan amount distribution, and more.
-   **Statistical Analysis:** Performed T-tests, Chi-square tests, and built a Logistic Regression model to identify significant predictors of loan default.
-   **Tableau Export:** Prepared aggregated data for Tableau, including default rates by state, year, grade, and purpose.

