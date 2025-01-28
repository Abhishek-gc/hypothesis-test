# E-commerce Delivery Time Analysis using Central Limit Theorem (CLT)

This project demonstrates how the **Central Limit Theorem (CLT)** can be used to estimate the average delivery time for orders in an e-commerce company, even when the raw data is highly skewed. The analysis includes:

1. **Synthetic Data Generation**: Simulates delivery times with a mix of normal and delayed orders.
2. **Central Limit Theorem (CLT) Simulation**: Repeatedly samples the data to show how sample means form a normal distribution.
3. **Confidence Interval Calculation**: Computes a 95% confidence interval for the true average delivery time.
4. **Interactive Visualizations**: Uses Plotly to create interactive graphs for better understanding.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Key Metrics](#key-metrics)
3. [Code Explanation](#code-explanation)
4. [Visualizations](#visualizations)
5. [How to Run the Code](#how-to-run-the-code)
6. [Dependencies](#dependencies)
7. [Summary for Non-Technical Stakeholders](#summary-for-non-technical-stakeholders)

---

## **Project Overview**

The goal of this project is to estimate the **average delivery time** for orders in an e-commerce company. The raw delivery time data is highly skewed, with most orders delivered in 2 days but some delayed up to 10 days. Using the **Central Limit Theorem (CLT)**, we show how to reliably estimate the true average delivery time and calculate a **95% confidence interval** for it.

---

## **Key Metrics**

- **True Average Delivery Time**: The actual average delivery time across all orders.
- **Natural Variation (Standard Deviation)**: Measures how much delivery times vary.
- **Sample Mean of Means**: The average of all sample means (should match the true average).
- **Standard Error**: Measures the precision of the sample mean estimate.
- **95% Confidence Interval**: A range where we are 95% confident the true average lies.

---

## **Code Explanation**

The code is divided into the following sections:

1. **Synthetic Data Generation**:
   - Creates a dataset of delivery times with a mix of normal (2 days) and delayed (10 days) orders.
   - Uses `np.random.normal` and `np.clip` to simulate realistic delivery times.

2. **Central Limit Theorem (CLT) Simulation**:
   - Repeatedly samples the data to calculate sample means.
   - Demonstrates how the distribution of sample means becomes normal, even with skewed data.

3. **Confidence Interval Calculation**:
   - Computes a 95% confidence interval using the sample mean and standard error.

4. **Interactive Visualizations**:
   - Uses Plotly Express to create interactive histograms for:
     - The original delivery time distribution.
     - The distribution of sample means (CLT in action).

---

## **Visualizations**

### 1. Original Delivery Times Distribution
- Shows the raw delivery time data, which is highly skewed.
- Includes a red dotted line for the true average delivery time.

### 2. Distribution of Sample Means (CLT)
- Shows how the sample means form a normal distribution.
- Includes:
  - A red dotted line for the true average.
  - A blue dashed line for the average of sample means.
  - A green shaded region for the 95% confidence interval.

---

## **How to Run the Code**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ecommerce-delivery-analysis.git
   cd ecommerce-delivery-analysis
