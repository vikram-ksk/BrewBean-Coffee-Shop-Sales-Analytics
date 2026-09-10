# BrewBean Coffee Shop Sales Analytics

## Project Overview
BrewBean Coffee Shop Sales Analytics is a Business Analytics project focused on analyzing sales performance, customer behaviour, product performance, promotional campaigns, and outlet operations for BrewBean Café.
The project uses Excel to clean, validate, analyze, and visualize business data and develop an interactive executive dashboard for management decision-making.

## Business Problem

BrewBean operates multiple coffee shop outlets across Tamil Nadu. The business is experiencing increasing footfall but inconsistent sales, varying outlet performance, peak-hour congestion, and fluctuating profitability.
The objective of this project is to identify key business trends and provide data-driven recommendations to improve sales performance, operational efficiency, profitability, and customer satisfaction.

## Objectives

- Analyze revenue and profit performance across outlets
- Identify top-selling products
- Identify peak/busiest business hours
- Evaluate promotional campaign performance
- Analyze revenue by customer membership segment
- Identify preferred payment methods
- Identify highly rated products
- Identify outlets requiring operational improvement
- Provide evidence-based business recommendations

## Dataset

The project uses five datasets:

1. Sales Transactions
2. Inventory
3. Product Master
4. Outlet Master
5. Promotions

## Data Cleaning

The following data preparation activities were performed:

- Removed duplicate Transaction_ID records
- Standardized Membership values
- Standardized Payment Mode values
- Standardized Transaction Date format
- Checked missing values
- Validated Quantity, Selling Price, Revenue and Profit
- Validated product selling price and profit margin
- Validated outlet master data
- Validated promotion dates and discount values
- Validated inventory stock records
- Created a `Sales_Valid` field to identify completed and cancelled transactions

Cancelled transactions were excluded from sales KPIs and business analysis.

## Data Modeling

Microsoft Power Pivot was used to create the Data Model.

### Relationships

- Product → Sales using Product_ID
- Outlet → Sales using Outlet_ID
- Product → Inventory using Product_ID
- Outlet → Inventory using Outlet_ID

The Promotions table was kept separate because the Applicable_Outlets field contains multi-value applicability and campaign usage was not complete enough for a direct relationship.

## Analysis Performed

### 1. Outlet Performance

Analyzed Revenue, Profit and Completed Transactions by outlet.

**Highest Revenue Outlet:** BrewBean Peelamedu — ₹28,311.16

**Highest Profit Outlet:** BrewBean Peelamedu — ₹17,504.16

### 2. Top-Selling Products

Analyzed product sales using Quantity.

**Top Product:** Product 50 — 59 units

### 3. Busiest Hours

Created a Transaction_Hour field using Transaction_Time and analyzed completed transactions by hour.

**Peak Hour:** 9 AM — 78 transactions

**Main Busy Period:** 7 AM–10 AM

### 4. Promotion Performance

Analyzed promotion-linked revenue.

**Top Promotion:** Weekend Family Combo — ₹41,437.30

### 5. Customer Membership Revenue

Analyzed revenue by Membership.

**Highest Revenue Segment:** Silver — ₹47,279.03

### 6. Payment Method Analysis

Analyzed completed transactions by payment method.

**Most Used Payment Method:** Google Pay — 177 transactions

### 7. Product Ratings

Analyzed average customer ratings by product.

**Highest Rated Product:** Product 19 — 4.50/5

### 8. Operational Improvement

Compared outlet Revenue, Profit and Completed Transactions.

**Priority Outlet:** BrewBean Salem

- Revenue: ₹16,450.17
- Profit: ₹9,782.17
- Completed Transactions: 45

## Executive Dashboard

An interactive Excel dashboard was developed containing:

- Total Revenue KPI
- Total Profit KPI
- Completed Transactions KPI
- Outlet Revenue & Profit
- Top 5 Products
- Transactions by Hour
- Promotion Revenue
- Revenue by Membership
- Payment Method Usage
- Top 5 Rated Products
- Interactive Outlet Slicer

## Key Business Recommendations

1. Increase staffing and service capacity during the 7 AM–10 AM peak period.
2. Prioritize BrewBean Salem for operational performance review.
3. Continue and optimize the Weekend Family Combo promotion.
4. Maintain sufficient stock and visibility for high-demand products.
5. Promote highly rated products to improve customer engagement and satisfaction.
6. Use the interactive dashboard for continuous outlet performance monitoring.

## Tools & Technologies

- Microsoft Excel
- Power Query
- Power Pivot
- PivotTables
- PivotCharts
- Excel Slicers
- Data Cleaning
- Data Validation
- Business Analytics
- Data Visualization

## Project Deliverables

- Raw datasets
- Cleaned datasets
- Excel analysis workbook
- Interactive executive dashboard
- Business analysis presentation
- Business insights and recommendations


## Conclusion

The analysis provides a structured view of BrewBean's sales, products, customers, promotions, payment behaviour, and outlet performance.

The insights help management identify peak-hour requirements, high-performing products and promotions, customer preferences, and outlets requiring operational attention.

The interactive Excel dashboard enables stakeholders to explore the results and support data-driven business decisions.
