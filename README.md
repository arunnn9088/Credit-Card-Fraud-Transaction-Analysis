# Credit-Card-Fraud-Transaction-Analysis
Statistical analysis and visualization of credit card transaction data to identify patterns in fraudulent activities using R and data analytics techniques.
# Credit Card Fraud Detection using Statistical Analysis

## Overview
Credit card fraud is a major challenge for financial institutions. Fraudulent transactions cause significant financial losses and require advanced analytical methods to detect suspicious activities.

This project analyzes credit card transaction data using statistical techniques and data visualization to identify patterns related to fraudulent transactions.

The goal is to understand transaction behavior and explore indicators that may help detect fraudulent activity.

---

## Dataset

The dataset contains credit card transaction records including customer information, merchant details, transaction amounts, and fraud indicators.

### Key Features

- **amt** – Transaction amount  
- **category** – Merchant category  
- **city_pop** – Population of the city  
- **lat / long** – Customer location  
- **merch_lat / merch_long** – Merchant location  
- **unix_time** – Transaction timestamp  
- **dob** – Customer date of birth  
- **is_fraud** – Fraud indicator (0 = normal transaction, 1 = fraudulent transaction)

---

## Data Preprocessing

Several preprocessing steps were applied to prepare the dataset for analysis:

1. **Unix timestamp conversion**
   - Converted `unix_time` into a readable datetime format.

2. **Feature extraction**
   - Extracted hour, day, and month from transaction timestamps.

3. **Data type corrections**
   - Converted `is_fraud` variable into numeric format.

4. **Data cleaning**
   - Removed formatting issues in timestamp fields.

---

## Exploratory Data Analysis

The project uses various visualization techniques to explore the dataset.

### Fraud Distribution
Bar charts were used to visualize the imbalance between fraudulent and non-fraudulent transactions.

### Box Plot Analysis
Box plots were used to compare transaction amounts between fraud and non-fraud transactions.

### Scatter Plot Analysis
Scatter plots were used to analyze relationships between transaction amount and city population.

### Histogram
Histograms were used to understand the distribution of transaction amounts.

---

## Statistical Analysis

The following statistical techniques were used:

- Descriptive statistics
- Normality testing (Shapiro-Wilk test)
- Hypothesis testing (T-test)
- Regression analysis

These techniques help identify patterns and differences between fraudulent and legitimate transactions.

---

## Key Findings

- Fraud transactions represent a very small percentage of total transactions.
- Transaction amounts vary widely across the dataset.
- Fraud transactions often show higher variability in transaction amounts.
- Transaction behavior may differ across geographic regions.

---

## Technologies Used

- R Programming
- Google Colab
- ggplot2
- dplyr
- lubridate
- corrplot

---

## Project Structure

```
data/           Dataset used for analysis
notebook/       Jupyter notebook containing analysis code
images/         Visualization outputs
report/         Project report
```

---

## Future Improvements

Future work may include:

- Machine learning models for fraud prediction
- anomaly detection algorithms
- real-time fraud detection systems

---

## Author

Data Analytics Project – Credit Card Fraud Detection
