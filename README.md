# South African Retail Sales Analysis

## Project Overview

This project analyses retail transaction data to identify patterns in
sales performance, customer purchasing behaviour, product categories,
sales channels, pricing, and discounts.

The project combines **Python and SQL**. SQL was used for core business
questions and window-based analysis, while Python, pandas, and
Matplotlib were used for deeper analysis and visualization.

## Business Questions

1.  Which products are purchased the most?
2.  How are discounts associated with quantity purchased?
3.  Is unit price associated with quantity purchased?
4.  Which products are purchased most in each city?
5.  Which product categories generate the strongest sales performance?
6.  How does revenue change throughout the year?
7.  How does customer purchasing behaviour differ?
8.  How do sales channels compare?
9.  How do discount levels relate to sales volume and revenue per order?

## Dataset

The final cleaned dataset contains **3,500 transaction records** with
order, customer, product, category, quantity, price, discount, city,
sales-channel, and date information.

### Data Quality

Initial exploration identified 10 duplicate rows, invalid quantity
values, currency-formatted prices, invalid date entries, inconsistent
text formatting, and missing values in quantity, order date, and city.
Records that remained useful for other analyses were retained where
appropriate.

## Tools & Technologies

-   Python
-   pandas
-   NumPy
-   Matplotlib
-   SQL
-   SQLite
-   Jupyter Notebook

SQL techniques include aggregations, `GROUP BY`, CTEs, window functions,
`RANK()`, and `NTILE()`.

## Key Findings

### Electronics Dominates Category Revenue

Electronics generated approximately **R13.57 million in revenue** and
also led in total quantity sold and number of orders. Furniture was the
second-highest revenue category at approximately **R4.12 million**.

### Store vs Mobile App

**Store** generated the highest total revenue at approximately **R7.20
million**, narrowly exceeding Mobile app at approximately **R7.18
million**. However, **Mobile app recorded the highest number of orders
(1,198)** compared with **1,161 Store orders**.

Product-level analysis indicated that Store transactions included
greater sales of higher-value products, contributing to its higher
average transaction value.

### Monthly Revenue Performance

-   **Highest revenue:** July --- approximately R1.95 million
-   **Lowest revenue:** May --- approximately R1.56 million
-   July revenue was approximately **25.1% higher than May revenue**

July also recorded more orders and units sold than May, alongside a
moderately higher average revenue per order.

### Customer Revenue Concentration

The **top 10 customers contributed approximately 6.1% of total
revenue**, indicating that the highest-revenue customers accounted for a
relatively small share of overall revenue.

### Discount Behaviour

Average quantity increased from approximately **2.17 units at 0%
discount to 2.65 units at 25% discount**, while average revenue per
order generally declined from approximately **R6,628 to R5,411**.

This indicates an observed trade-off between **sales volume and revenue
per transaction**. Product-level analysis showed that no single discount
level consistently produced the highest observed average revenue per
order across all products.

### City-Level Product Performance

  City           Most Purchased Product
  -------------- ------------------------
  Bloemfontein   Sneakers
  Cape Town      Tablet
  Durban         Kettle
  Gqeberha       Smartphone
  Johannesburg   Sneakers
  Pretoria       Desk

## Visual Analysis

The notebook includes visualizations for monthly revenue, sales-channel
revenue and orders, category revenue, and discount behaviour.

## Conclusion

Retail performance varies across categories, channels, customers, and
discount levels. **Electronics is the strongest revenue-generating
category**, while Store and Mobile app show different strengths: Store
generates slightly greater revenue and higher-value transactions,
whereas Mobile app leads in transaction volume.

Higher discounts are generally associated with greater quantities
purchased per order, but not necessarily greater revenue per
transaction. Because this is observational transaction data, these
results identify associations rather than proving causal effects.

## Repository Structure

``` text
retail-sales-analysis/
├── data/
│   └── retail_sales_project_2.csv
├── notebooks/
│   └── Retail-sales-project-polished.ipynb
└── README.md
```

## Skills Demonstrated

**Data Analysis:** Data cleaning, EDA, aggregation, customer analysis,
pricing analysis, and business interpretation

**Python:** pandas, NumPy, Matplotlib

**SQL:** SQLite, `GROUP BY`, aggregations, CTEs, `RANK()`, `NTILE()`,
and window functions

**Visualization:** Business-focused charts and insight communication
