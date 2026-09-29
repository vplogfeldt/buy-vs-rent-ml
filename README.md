# buy-vs-rent-ml
Project focused on comparing housing costs

## 📌 Project Overview

This project builds a decision-support tool that helps users compare the long-term financial consequences of buying versus renting residential property. By combining machine learning for property valuation with economic simulations, the application provides data-driven financial insights over custom time horizons.

The project integrates:
* **Statistics & EDA:** Exploratory data analysis of the housing market in R.
* **Machine Learning:** Predictive models for property valuation.
* **Economic Simulation:** Scenario testing (Buy vs. Rent) accounting for opportunity costs and interest rates.
* **Web Application & API:** An interactive interface for end users.

---

## 🎯 Objectives & Core Questions

* **Primary Question:** Can housing market data be leveraged to train a predictive model that accurately estimates property prices?
* **Long-term Goal:** Combine the price estimation model with a financial simulation engine to calculate total cost, net worth development, and opportunity costs over flexible timeframes and interest rate scenarios.

---

## 🚦 Project Status (Month 1 of 4)

The project is currently in Phase 1, focusing on **Statistics, R, and ML Fundamentals**:
- [x] Set up project structure and version control
- [/] Identify and evaluate a suitable housing dataset
- [ ] Perform exploratory data analysis (EDA)
- [ ] Train a baseline linear regression model

---

## 📊 Data & Variables

*Dataset and source will be finalized during Month 1.*

| Variable | Description | Data Type |
| :--- | :--- | :--- |
| `price` | Property price (Target) | *TBD* |
| `area` | Living area in square meters ($m^2$) | *TBD* |
| `rooms` | Number of rooms | *TBD* |
| `location` | Geographic region / Area | *TBD* |
| `fee` | Monthly fee to association / landlord | *TBD* |

> *This table will be updated once the dataset is selected and validated.*

---

## 🔍 Exploratory Data Analysis (EDA) & Modeling

### EDA
Month 1 analysis focuses on:
* Price distribution and outlier detection.
* Price per square meter relative to geographic location.
* Correlations between features (`area`, `rooms`, `fee` vs. `price`).

### Model Development
The initial baseline model is a **Linear Regression**:
$$\text{Price} = \beta_0 + \beta_1(\text{Area}) + \beta_2(\text{Rooms}) + \beta_3(\text{Fee}) + \epsilon$$

*Model performance metrics ($R^2$, RMSE) and visualizations will be added continuously.*

---

## 📂 Project Structure

```text
.
├── README.md
├── data/
│   ├── raw/          # Raw data (git-ignored if large)
│   └── processed/    # Cleaned and transformed data
├── R/
│   ├── 01_import.R   # Data ingestion and cleaning
│   ├── 02_eda.R      # Exploratory data analysis and charts
│   └── 03_model.R    # Linear regression and modeling
├── notebooks/        # RMarkdown / Quarto documents
├── figures/          # Exported plots and visualizations
└── models/           # Saved trained models (.rds / .RData)