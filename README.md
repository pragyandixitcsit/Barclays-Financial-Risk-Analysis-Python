# Barclays Financial Risk Analysis with Python

## Project Description

This project focuses on analyzing Barclays financial transactional data using Python to understand customer financial behavior, transaction patterns, account activity, and potential financial risks.

The analysis includes data cleaning, descriptive transaction analysis, customer profiling, financial risk identification, exploratory data analysis, anomaly detection, and hypothesis testing.

The project aims to generate data-driven insights that can support customer engagement strategies and financial risk monitoring.

---

## Project Objectives

- Clean and preprocess financial transaction data.
- Analyze credit, debit, and net transaction trends.
- Identify high-performing and low-performing accounts.
- Detect dormant or inactive accounts.
- Build customer profiles based on transaction activity and balances.
- Identify potentially risky financial behavior.
- Detect transaction and balance anomalies.
- Perform exploratory data analysis using visualizations.
- Conduct hypothesis testing on transaction volume and average account balance.
- Generate actionable business insights and recommendations.

---

## Dataset

**Dataset:** Barclays Financial Transactional Data

The dataset contains customer and account-level transactional information such as:

- Transaction ID
- Customer ID
- Account ID
- Account Type
- Transaction Type
- Product
- Firm
- Region
- Manager
- Transaction Date
- Transaction Amount
- Account Balance
- Risk Score
- Credit Rating
- Tenure Months

The project brief describes the dataset as a transactional summary containing account information, transaction dates, transaction types, transaction amounts, account types, and available balances.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- Statistical Analysis
- Exploratory Data Analysis (EDA)

---

## Project Workflow

### 1. Data Cleaning and Formatting

- Cleaned financial fields.
- Converted transaction amounts into numerical format.
- Validated transaction dates.
- Standardized account and transaction categories.
- Checked the dataset for inconsistencies.

### 2. Descriptive Transactional Analysis

- Calculated monthly transaction summaries.
- Calculated yearly transaction summaries.
- Analyzed total credits and debits.
- Calculated net transaction volume.
- Analyzed account-level net inflow.
- Identified dormant/inactive accounts.
- Visualized transaction trends over time.

### 3. Customer Profile Building

Customers/accounts were analyzed based on:

- Transaction frequency
- Average account balance
- Transaction volume
- Net inflow

Activity levels were classified into:

- High Activity
- Medium Activity
- Low Activity

Additional profiles included:

- High-net-inflow accounts
- High-frequency low-balance accounts
- Negative or near-zero balance accounts

### 4. Financial Risk Identification

The project analyzed:

- Frequent large withdrawals
- Overdraft occurrences
- Balance volatility
- Statistical anomalies
- Irregular transaction behavior

Anomaly detection was performed using statistical techniques such as:

- Interquartile Range (IQR)
- Z-score based analysis

### 5. Exploratory Data Analysis

Multiple visualizations were created to understand:

- Transaction trends
- Credit vs debit activity
- Account activity
- Customer segments
- Balance behavior
- Financial risk indicators
- Transaction patterns

### 6. Hypothesis Testing

The project tested whether high-volume transaction accounts have statistically higher average balances than low-volume transaction accounts.

Statistical testing was performed using customer/account segmentation and average balance comparison.

---

## Key Analysis Results

| Metric | Result |
|---|---:|
| Total Transactions | 800 |
| Unique Accounts | 193 |
| Dormant/Inactive Accounts | 166 |
| High Activity Accounts | 37 |
| Medium Activity Accounts | 113 |
| Low Activity Accounts | 43 |
| High Net-Inflow Accounts | 49 |
| High-Frequency Low-Balance Accounts | 76 |
| Overdraft Accounts | 14 |
| IQR Anomalies | 7 |
| Average Risk Score | 0.4726 |

---

## Hypothesis Testing Result

The analysis compared average balances between high-volume and low-volume transaction accounts.

**High-volume average balance:** 71,919.57

**Low-volume average balance:** 74,829.28

**p-value:** 0.2258

Based on the statistical test performed in the project, the observed difference was not statistically significant at the conventional 5% significance level.

---

## Key Insights

- A significant number of accounts showed periods of inactivity based on the defined transaction-gap criteria.
- Customer accounts displayed different levels of transaction activity.
- High-frequency low-balance accounts were identified as an important segment for financial monitoring.
- Overdraft accounts and large withdrawal patterns provided potential risk indicators.
- Statistical anomaly detection helped identify unusual transaction or balance behavior.
- Transaction volume alone did not show a statistically significant difference in average balances between the high-volume and low-volume groups.

---

## Business Recommendations

1. **Monitor high-frequency low-balance accounts**

   Accounts with frequent transactions but relatively low balances can be monitored for potential liquidity or financial stress indicators.

2. **Strengthen monitoring of overdraft activity**

   Accounts with repeated overdrafts or large withdrawals can be prioritized for additional risk monitoring.

3. **Use customer segmentation**

   Activity, balance, and transaction-volume segments can be used to design more targeted customer engagement and monitoring strategies.

4. **Apply anomaly detection regularly**

   Statistical techniques such as IQR and Z-score analysis can help identify unusual transaction patterns.

---

## Project Structure

```text
barclays-financial-risk-analysis-python/
│
├── PythonProject.ipynb
├── Barclays_Financial_Risk_Analysis.pdf
├── Barclays_Financial_Transactional_Data.csv
├── README.md
└── requirements.txt
