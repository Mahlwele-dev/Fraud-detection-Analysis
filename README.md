# Fraud Detection Analytics Project

## Overview
This project focuses on analyzing financial transaction data to identify fraudulent behavior and suspicious transaction patterns using Python, PostgreSQL, SQL, and Power BI.

The project follows a complete end-to-end analytics workflow including:
- Data loading and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering
- SQL-based fraud investigation
- Interactive dashboard development
- Business reporting and presentation

The main objective of the project was to investigate fraudulent transaction behavior, identify high-risk transaction patterns, and generate business insights for fraud monitoring and operational decision-making.

---

# Dataset

The dataset contains transactional financial records used for fraud detection analysis.

## Features Included
- `step` – Hourly transaction time step
- `type` – Transaction type
- `amount` – Transaction amount
- `nameOrig` – Sender account
- `oldbalanceOrg` – Sender balance before transaction
- `newbalanceOrig` – Sender balance after transaction
- `nameDest` – Receiver account
- `oldbalanceDest` – Receiver balance before transaction
- `newbalanceDest` – Receiver balance after transaction
- `isFraud` – Fraud indicator
- `isFlaggedFraud` – Flagged suspicious transaction indicator

---

# Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and preprocessing |
| Pandas | Data manipulation |
| PostgreSQL | Database storage |
| SQL | Fraud investigation queries |
| Power BI | Dashboard creation |
| Gamma | Presentation creation |
| Jupyter Notebook | Development environment |

---

# Project Workflow

## 1. Data Loading & Exploration
The dataset was loaded into Python using Pandas for initial analysis.

### Tasks Performed
- Checked dataset structure
- Reviewed column information
- Generated summary statistics
- Investigated fraud distribution
- Checked for missing values and duplicates

---

## 2. Data Cleaning
Performed data quality and consistency checks.

### Cleaning Steps
- Checked for null values
- Verified duplicate records
- Investigated zero-value transactions
- Checked for negative balances
- Standardized data formatting

---

## 3. Feature Engineering
Created additional features to support fraud analysis.

### Features Created
- `HoursOfDay`
- `errorBalanceOrig`
- `errorBalanceDest`
- Fraud status labels
- Balance consistency indicators

### Balance Consistency Logic
<img width="1778" height="380" alt="image" src="https://github.com/user-attachments/assets/11a663e0-2da7-4905-b74e-20cac7a948db" />


These engineered features helped identify suspicious balance discrepancies and transaction anomalies.

---

# SQL Business Questions

The cleaned dataset was loaded into PostgreSQL to answer business-focused fraud investigation questions.

## Key Questions Investigated
1. Which destination accounts received the most stolen money?
2. Which transaction types are most associated with fraud?
3. At what hours does fraud occur most frequently?
4. Are balance inconsistencies linked to fraudulent transactions?
5. Which accounts display repeated suspicious behavior?

---

# Power BI Dashboard

An interactive dashboard was created in Power BI to visualize fraud trends and operational risks.

## Dashboard Highlights
- Fraud vs Non-Fraud overview
- Fraud by transaction type
- Fraud percentage by hour
- Transaction activity trends
- Balance inconsistency analysis
- Interactive slicers and filters

## Dashboard Features
- KPI cards
- Multi-page dashboard design
- Time-based fraud analysis
- Interactive filtering
- Anomaly-focused visualizations

---

# Key Findings

- Fraud activity was heavily concentrated in `TRANSFER` and `CASH_OUT` transaction types.
- Certain destination accounts repeatedly received high-value fraudulent transactions.
- Fraud activity showed unusual concentration during lower operational hours.
- Balance inconsistencies revealed suspicious transaction behavior and reconciliation anomalies.
- Multiple accounts displayed repetitive transaction structures and suspicious financial patterns.

---

# Business Recommendations

- Improve monitoring of high-risk destination accounts.
- Increase fraud detection controls during high-risk operational hours.
- Strengthen balance reconciliation procedures.
- Implement anomaly detection rules for suspicious transaction behavior.
- Enhance monitoring for repeated high-value transaction activity.

