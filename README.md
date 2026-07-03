# Exploratory-Data-Analysis-EDA-Project-2
## Overview

This notebook performs **Exploratory Data Analysis (EDA)** on an e-commerce dataset to understand its structure, identify trends, summarize important statistics, and detect unusual observations before further analysis or modeling.

The analysis is implemented using the **Pandas** library and follows a structured workflow from data inspection to outlier detection.

## Objectives

The notebook aims to:

* Explore the dataset's structure and dimensions.
* Generate descriptive statistics for numerical variables.
* Analyze product performance and marketing channels.
* Examine monthly sales and order trends.
* Detect abnormal transactions using the Interquartile Range (IQR) method.

## Workflow Summary

### 1. Descriptive Statistics

Summary statistics are generated for numerical variables to understand their distributions. Additional aggregation is performed to calculate the mean, median, and total number of observations for important business metrics such as:

* Quantity
* Unit Price
* Items in Cart
* Total Price

### 2. Product and Marketing Analysis

The notebook evaluates product performance by calculating:

* Total revenue generated
* Average customer spending
* Total quantity sold
* Number of orders

Products are ranked according to their revenue contribution.

Marketing channels (Referral Sources) are also analyzed to determine which platforms contribute the highest sales revenue.

### 3. Time-Series Analysis

The transaction date is converted into a datetime format, allowing monthly aggregation of sales data.

Monthly analysis includes:

* Total monthly revenue
* Monthly order volume

This helps identify overall business growth and seasonal sales patterns.

### 4. Outlier Detection

The notebook applies the **Interquartile Range (IQR)** method to identify unusually large or small transaction values.

The process includes:

* Calculating the first and third quartiles (Q1 and Q3)
* Computing the Interquartile Range (IQR)
* Defining lower and upper outlier boundaries
* Extracting transactions outside these limits
* Displaying summary information and the highest-value outlier transactions

## Libraries Used

* **Pandas** – Data loading, manipulation, aggregation, and statistical analysis.

## Expected Outcomes

After completing the notebook, users can:

* Understand the overall structure of the dataset.
* Summarize important business metrics.
* Identify top-performing products.
* Evaluate the effectiveness of referral sources.
* Observe monthly revenue and order trends.
* Detect and investigate abnormal transactions for further analysis.

---

## Conclusion

This EDA notebook provides a comprehensive overview of the e-commerce dataset by combining statistical summaries, business-oriented aggregations, temporal trend analysis, and outlier detection. The insights generated during this stage establish a strong foundation for subsequent data cleaning, visualization, predictive modeling, and business decision-making.
