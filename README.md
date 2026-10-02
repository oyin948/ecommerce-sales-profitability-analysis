# E-Commerce Sales & Profitability Analysis

## Project Overview

This project analyzes e-commerce sales and profitability data to identify the main revenue and profit drivers, highlight loss-making sub-categories, and examine differences in profitability across payment methods.

The analysis was completed in **Power BI** using **DAX** measures and an interactive dashboard.

---

## Business Questions

The analysis was designed to answer the following questions:

1. What are the overall revenue, profit, profit margin, and quantity sold?
2. Which categories contribute the most revenue and profit?
3. Which sub-categories generate the highest and lowest profit?
4. Does higher sales volume necessarily translate into higher profit?
5. Which payment methods are associated with higher profitability?
6. Which areas should management investigate to improve profitability?

---

## Headline Results

- **₹437,771** total revenue
- **₹36,963** total profit
- **8.44%** overall profit margin
- **5,615** units sold across **500 unique orders**
- **Clothing** recorded the highest quantity sold and the highest category-level profit.
- **Electronics** generated the highest category-level revenue.
- **Printers** generated the highest sub-category profit at **₹8,606**.
- **Five sub-categories** recorded negative profit, with **Furnishings** recording the largest loss at **-₹806**.
- **Credit Card (CC)** transactions recorded the highest profit (**₹12,612**) and highest profit margin (**15%**) among the payment modes.

[Dashboard.png](Screenshot/Dashboard.png)

---

## Dataset

The dataset contains **1,500 order line items representing 500 unique customer orders in India**.

### Variables

| Variable | Description |
|---|---|
| `order_id` | Customer order identifier |
| `amount` | Revenue generated from the transaction |
| `profit` | Profit generated from the transaction |
| `quantity` | Quantity of products sold |
| `category` | Main product category |
| `sub_category` | Product sub-category |
| `payment_mode` | Payment method used |

### Dataset Link

[View/download the project dataset](Data/Details_cleaned.xlsx)

---

## Tools Used

- **Power BI** — data analysis and dashboard development
- **DAX** — KPI and profitability calculations

---

## Analysis Performed

- Overall sales and profitability analysis
- Sub-category profitability analysis
- Identification of loss-making sub-categories
- Payment-mode profitability analysis
- Comparison of quantity sold with profit
- Interactive dashboard development

### Key Measures

- Total Revenue
- Total Profit
- Total Quantity
- Profit Margin

---

## Key Insights

### 1. High sales volume does not necessarily mean high profitability

Saree recorded the highest quantity sold at **795 units**, while Printers generated the highest profit at **₹8,606**.

This shows that sales volume alone is not sufficient for evaluating sub-category performance.

### 2. Several sub-categories generated losses

Five sub-categories recorded negative profit:

| Sub-category | Profit |
|---|---:|
| Furnishings | -₹806 |
| Electronic Games | -₹644 |
| Kurti | -₹401 |
| Skirt | -₹315 |
| Leggings | -₹130 |

Furnishings is particularly notable because it sold **310 units** while still generating a loss.

### 3. Category performance differs by metric

| Category | Quantity | Revenue | Profit |
|---|---:|---:|---:|
| Clothing | 3,516 | ₹144,323 | ₹13,325 |
| Electronics | 1,154 | ₹166,267 | ₹13,162 |
| Furniture | 945 | ₹127,181 | ₹10,476 |

Clothing recorded the highest quantity and profit, while Electronics generated the highest revenue. This demonstrates why revenue, quantity, and profit should be considered together.

### 4. Payment modes show differences in profitability

| Payment Mode | Quantity | Revenue | Profit | Profit Margin |
|---|---:|---:|---:|---:|
| COD | 2,456 | ₹155,181 | ₹12,547 | 8% |
| CC | 672 | ₹86,932 | ₹12,612 | 15% |
| DC | 741 | ₹49,136 | ₹3,694 | 8% |
| EMI | 589 | ₹77,881 | ₹4,824 | 6% |
| UPI | 1,157 | ₹68,641 | ₹3,286 | 5% |

CC recorded the highest profit and profit margin despite having substantially lower quantity than COD.

These results indicate an **association** between payment mode and profitability in this dataset; they do not establish that payment method itself causes higher or lower profit.

---

## Recommendations

1. **Review loss-making sub-categories.**  
   Investigate pricing, costs, discounts, and other available factors behind negative-profit sub-categories, particularly Furnishings.

2. **Evaluate products using both volume and profit.**  
   High sales volume should not automatically be treated as strong performance if the resulting profit is low or negative.

3. **Investigate Electronics' revenue-to-profit performance.**  
   Electronics generated the highest category revenue but slightly less profit than Clothing. Reviewing its pricing and cost structure could help explain the difference.

4. **Examine payment-mode profitability.**  
   Investigate the factors behind differences in profitability across payment modes, including whether transaction size or product mix contributes to the observed differences.

5. **Monitor revenue, quantity, and profit together.**  
   Future reporting should use multiple profitability measures rather than relying on sales volume or revenue alone.

---

## Limitations

- The dataset does not contain detailed product-level cost, pricing, discount, or customer demographic information, limiting the ability to explain the causes of some profitability differences.
- The analysis identifies associations and patterns in the available data; it does not establish causal relationships.
- The dataset covers the transactions provided for this challenge and may not represent a broader or longer business period.
- The analysis is limited to the variables available in the dataset, so other operational factors that may influence profitability are not captured.

---

## Dashboard

The interactive Power BI dashboard includes:

- Total Revenue
- Total Profit
- Profit Margin
- Total Quantity
- Revenue and Profit by Category
- Profit by Sub-category
- Profit by Payment Mode
- Quantity vs Profit scatter analysis
- Sub-category profitability table
- Category filter

### Dashboard Link

[View the project dashboard and Power BI files](Screenshot/Dashboard.png/)

The repository contains the Power BI `.pbix` file, dataset, screenshots, and project documentation.

---

## Project Structure

```text
E-Commerce-Sales-Profitability-Analysis/
│
├── Data/
│   └── Details_cleaned.csv
│
├── PowerBI/
│   └── E-Commerce Sales Profitability Analysis.pbix
│
├── Screenshot/
│   └── Dashboard.png
│
└── README.md
```

---

## Author

**Oyindamola**

Data Science Student | Aspiring Data Analyst

- **GitHub:** https://github.com/oyin948
- **Email:** oladejoaisha7@gmail.com
- **X:** [https://x.com/AishatOyinda]
