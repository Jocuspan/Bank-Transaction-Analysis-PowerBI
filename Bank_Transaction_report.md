### Bank Transaction Data Analyst Dashboard | Power BI

#### Project Overview

This project uses Power BI to analyze bank transaction data, focusing on transaction patterns, fraudulent activities, fraud detection performance, transaction types, and account balance changes. This report employs visualizations such as KPI cards, line charts, donut charts, and waterfall charts to help users quickly analyze fraudulent activity in banking transactions.



#### Project Objectives

Monitor overall banking transaction performance through key performance indicators.

Identify transaction patterns and fraud trends across different time steps.

Explore the relationship between transaction amounts and account balance changes.

Evaluate fraud detection performance using Precision, Recall, and fraud flagging rates.

Identify suspicious destination accounts and analyze fraudulent transaction amounts.

Build an interactive dashboard to support fraud monitoring and risk analysis.



#### Data Modeling

FactTransactions: Main transaction data, including amounts, balances, time, and fraud indicators.

DimDestinationAccount: Destination account information.

DimFraudStatus: Fraud classification and status information.

DimOriginAccount: Origin account information.

DimTime: Transaction time attributes for time-based analysis.

DimTransactionType: Transaction categories for fraud and transaction analysis.



#### Dashboard Pages \& Analysis

Page 1 -- Bank Transaction Overview -- Overall transaction performance and fraud monitoring

Key visualizations:

KPI Cards: Total transaction count, total transaction amount, total fraud transactions, fraud rate, and total fraud amount.

Clustered Column Chart: Fraud rate comparison across different transaction types.

Fraud is an infrequent and high-impact issue, occurring almost exclusively within "transfer" and "cash-out" transactions. Monitoring efforts should focus on these two types of transactions, with stricter verification measures implemented for large-value transfers and unusual fluctuations in account balances.



Page 2 -- Fraud Transaction Analysis -- Fraud patterns, transaction trends, and account balance analysis

Key visualizations:

Line Chart: Fraud transaction trends by step group and transaction type.

Line and Bar Chart: Transaction amount distribution and fraud rate across different transaction amount groups.

Scatter Chart: Relationship between transaction amounts and origin account balance changes, with fraud status differentiation.

Interactive slicers for filtering sales data by transaction type.

Fraudulent transactions have long been a persistent problem, primarily occurring in large-value transactions and characterized by a discrepancy between changes in account balances and the actual transaction amounts. Stricter checks should be implemented for "Transfer" and "Cash Out" transactions, as these types are most frequently associated with fraudulent activity.



Page 3 -- Fraud Amount \& Account Analysis -- Fraud amount distribution and high-value transaction analysis

Key visualizations:

Donut Chart: Fraud amount distribution across different transaction types.

Bar Chart: Top 10 destination accounts ranked by transaction amount.

Fraud transaction is primarily concentrated in two types of transactions "Transfers" and "Cash Out," which occur with similar frequency with the funds ultimately flowing into a small number of accounts that receive large amount payments.



Page 4 -- Fraud Detection \& Balance Analysis -- Fraud detection performance and account balance changes

Key visualizations:

KPI Cards: Fraud detection rate and fraud flag rate.

Matrix: Comparison of actual fraud status and system-flagged fraud status.

Waterfall Charts: Origin account balance differences across transaction types.

Waterfall Charts: Destination account balance differences across transaction types.

The fraud detection rate is below 0.2%, despite zero false positives. Adjust alert thresholds, monitor large transfers and withdrawals, and verify transaction balance changes to improve detection while controlling false alarms.



#### Key Skills Demonstrated

Data Cleaning \& Transformation

Power Query (ETL)

DAX Measures \& Calculations

Data Modeling

Exploratory Data Analysis (EDA)

Fraud Detection \& Risk Analysis

Transaction Pattern Analysis

Data Visualization

Business Intelligence

KPI Development \& Performance Analysis



#### Final Conclusion

There were 8,213 fraudulent transactions, resulting in losses of approximately $12 billion; these were primarily concentrated in the "Transfer" and "Cash Out" categories. The fraudulent transactions involved significant sums and were accompanied by anomalous balance fluctuations. Currently, the system detects only 0.19% of such fraudulent activity. It is recommended that alert thresholds be adjusted, and that monitoring be strengthened for large-value transactions, high-risk recipient accounts, and unusual changes in account balances.

