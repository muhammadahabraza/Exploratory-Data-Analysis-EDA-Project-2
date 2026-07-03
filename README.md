# Exploratory-Data-Analysis-EDA-Project-2
## Order Patterns, Trends, and Distributions

This project focuses on the exploratory data analysis (EDA) of an e-commerce transactions dataset containing 1,200 unique order records spanning from January 2023 to June 2025. The core analysis outlines customer purchasing behaviors, statistical distributions, revenue trends, and key operational insights.

## 📊 Summary Statistics & Distributions
* **Dataset Size:** 1,200 unique transactions with 14 distinct features spanning transaction dates, product details, payment methods, and marketing channels.
* **Basket Metrics:** The average order contains approximately **3 units** of a single item, while the average comprehensive basket size (`ItemsInCart`) holds **5.5 items**.
* **Price Volatility:** `UnitPrice` ranges significantly from a minimum of **$11.39** up to **$699.93**, indicating a diverse inventory layout consisting of low-cost accessories and premium electronic hardware.
* **Revenue Skew:** 
  * **Mean Order Value:** $1,053.97
  * **Median Order Value:** $823.62
  * **Insight:** The notable variance between the mean and median indicates a right-skewed distribution. The average revenue is driven upward by a subset of premium, high-value transactions.

## 📈 Identified Trends & Outliers

### 1. Chronological Timeline
The dataset tracks longitudinal customer purchasing patterns starting on **January 1, 2023** and concluding on **June 30, 2025**. This 2.5-year window provides sufficient historical depth to run monthly or quarterly moving average reviews to track seasonal commercial fluctuations.

### 2. Coupon Utilization
During data preprocessing, it was revealed that **309 transactions** did not utilize a discount code. These records were systematically classified under a new distinct flag `NO_COUPON` to enable clean behavioral segmentation between price-sensitive (coupon-driven) shoppers and organic buyers.

### 3. Outlier Profile
While 75% of all client purchases fall beneath **$1,578.48**, the maximum transaction value recorded peaks at **$3,456.40**. Applying the Interquartile Range (IQR) rule identifies transactions pushing past the upper boundary as statistical revenue outliers—representing bulk corporate purchasing behaviors or high-end electronics bundles.

## 🚀 Technical Framework & Key Skills Applied

The analytical process in `Untitled21.ipynb` showcases the implementation of standard data science competencies:
* **Data Cleaning:** Missing value imputation (e.g., categorical padding of `CouponCode`), structural dimension testing (`df.shape`), and deduplication validations (`df.duplicated()`).
* **Descriptive Statistics:** Evaluation of central tendency (mean, median) and dispersion constraints (min, max, standard deviation) across continuous business variables.
* **Analytical Thinking:** Transforming raw log metrics into structured, clean distributions primed for trend charting and business strategy modeling.
