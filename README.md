# Procurement Management System

## Project Overview

This project focuses on analyzing **4,000+ procurement transaction records** using SQL and Tableau to identify inefficiencies in vendor management, inventory planning, and procurement spending.

The analysis was designed around a real-world procurement scenario commonly seen in construction, infrastructure, and supply chain operations, where delayed procurement decisions can directly affect project execution.

The main objective was to detect:

- Vendor concentration risks
- High-demand products requiring priority restocking
- Low-stock items below reorder thresholds
- Demand vs stock mismatches
- Monthly procurement spending fluctuations

This project demonstrates how data-driven procurement planning can reduce operational delays, improve vendor management, and strengthen inventory control.

---

## Problem Statement

Organizations often struggle with procurement inefficiencies because of:

- Heavy dependence on a few vendors
- Poor inventory replenishment planning
- Frequent shortages of high-demand products
- Unplanned emergency purchasing
- Large month-to-month spending fluctuations
- Weak demand forecasting

These issues lead to:

- Delayed project execution
- Increased procurement costs
- Budget forecasting issues
- Vendor dependency risks
- Supply chain inefficiencies

The goal of this project was to use SQL-based analysis to identify these issues and provide actionable insights for better procurement decision-making.

---

## Tools & Technologies Used

- MySQL (SQL Analysis)
- Tableau Public (Dashboard Visualization)
- Microsoft Excel / CSV
- GitHub

---

## Dataset Details

The dataset contains **4,000+ procurement transactions** across multiple vendors and products.

### Key Columns:

- Order ID
- Product ID
- Product Name
- Vendor ID
- Vendor Name
- Quantity
- Unit Price
- Total Cost
- Order Date
- Current Stock
- Reorder Level

This dataset was structured to simulate procurement operations relevant to construction and infrastructure projects.

---

## Key Analysis & Findings

---

## 1. Vendor Concentration Risk Analysis

### SQL Objective

Identify vendors contributing the highest procurement spend.

### Key Finding

Top vendors contributed the largest share of total procurement spend:

| Vendor Name | Total Spend |
|---|---:|
| AquaFlow Solutions | ₹10,258,481 |
| Bharat Infra Supply Co. | ₹9,740,426 |
| Shree Steel Traders | ₹9,640,290 |
| Reliable Bitumen Works | ₹9,602,658 |
| Green Earth Aggregates | ₹9,570,257 |

### Business Insight

The company showed strong dependency on a limited number of vendors, creating supplier concentration risk.

If one major vendor fails, procurement cycles and project execution may be affected significantly.

---

## 2. High-Demand Product Analysis

### SQL Objective

Identify products with the highest procurement demand.

### Key Finding

Top high-demand products:

| Product Name | Total Demand |
|---|---:|
| Electrical Cables | 55,098 |
| Bitumen Drums | 50,817 |
| Paver Blocks | 50,653 |
| PVC Drain Pipes | 50,422 |
| Stormwater Grates | 49,137 |

### Business Insight

These products require stronger replenishment planning because stockouts in these categories can directly delay operations.

---

## 3. Reorder Threshold Analysis

### SQL Objective

Identify products where current stock is below safe reorder levels.

### Key Finding

Critical low-stock products included:

| Product Name | Current Stock | Reorder Level |
|---|---:|---:|
| PVC Drain Pipes | 5 | 35 |
| Paver Blocks | 5 | 45 |
| Coarse Aggregates | 5 | 60 |
| Stormwater Grates | 5 | 20 |

### Business Insight

These items required urgent procurement attention to avoid stockouts and emergency purchasing costs.

---

## 4. Demand vs Stock Gap Analysis

### SQL Objective

Compare procurement demand with available stock.

### Key Finding

Severe demand-supply mismatch identified:

| Product Name | Total Demand | Avg Stock | Demand/Stock Ratio |
|---|---:|---:|---:|
| Electrical Cables | 55,098 | 61.9 | 889.75 |
| Bitumen Drums | 50,817 | 60.1 | 845.13 |
| Stormwater Grates | 49,137 | 59.4 | 827.03 |
| PVC Drain Pipes | 50,422 | 60.9 | 826.97 |
| Paver Blocks | 50,653 | 63.5 | 797.76 |

### Business Insight

Demand was significantly higher than available stock for critical products, showing weak inventory forecasting and reactive procurement planning.

---

## 5. Monthly Procurement Spending Trend

### SQL Objective

Track monthly procurement spending fluctuations.

### Key Finding

| Month | Monthly Spend |
|---|---:|
| February | ₹69,707,284 |
| March | ₹82,272,414 |
| October | ₹82,618,027 |
| December | ₹90,817,145 |

### Highest Spend Month

**December → ₹90.8M**

### Lowest Spend Month

**February → ₹69.7M**

### Business Insight

Significant monthly fluctuations indicated inconsistent procurement planning and the need for stronger budgeting and forecasting strategies.

---

## Tableau Dashboard

The dashboard includes:

- Top Vendors by Spend
- High-Demand Products
- Low Stock Alert Table
- Monthly Procurement Spending Trend

The dashboard was built using Tableau Public to visually present procurement risks and inventory decision points.

---

## SQL Queries Included

The full SQL script contains:

- Database creation
- Table creation
- Vendor concentration analysis
- Product demand analysis
- Reorder threshold detection
- Demand-stock ratio analysis
- Monthly spending trend analysis

Available in:

```text
sql/procurement_queries.sql
