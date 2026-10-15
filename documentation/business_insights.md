# NovaMart Retail — Business Insights & Recommendations

## 1. Project Overview

NovaMart Retail is a fictional multi-store retailer used to demonstrate business analysis, data quality validation, sales performance analysis, and inventory reporting.

This project uses synthetic data representing 1,000 transactions, 50 products, 10 stores, and 500 store-product inventory records for a simulated 2026 reporting period.

## 2. Key Business Metrics

| KPI                 |     Result |
| ------------------- | ---------: |
| Total Sales         | ₹45,08,300 |
| Total Profit        | ₹17,83,900 |
| Profit Margin       |     39.57% |
| Average Order Value |  ₹4,508.30 |
| Total Units Sold    |      3,000 |
| Total Transactions  |      1,000 |
| Inventory Records   |        500 |
| Low-Stock Records   |          0 |
| Overstock Records   |        107 |
| Overstock Rate      |     21.40% |

*All values are derived from synthetic data and are intended for portfolio demonstration.*

## 3. Sales Performance Insights

### Store Performance

* NovaMart Lucknow Central recorded the highest sales at ₹9,31,600 and the highest total profit at ₹3,31,600.
* NovaMart Pune Central recorded the lowest sales at ₹97,900.
* NovaMart Pune Central had the highest calculated profit margin at approximately 47.91%, while NovaMart Lucknow Central had the lowest at approximately 35.59%.

These differences should be interpreted cautiously because store and product assignments follow a repeating pattern in the synthetic transaction data.

### Product Performance

The three highest-revenue products were:

1. Vacuum Cleaner — ₹5,19,920
2. Air Fryer — ₹3,13,146
3. Food Processor — ₹2,92,332

These results demonstrate how product-level aggregation can help identify products contributing the most revenue in a dataset.

## 4. Inventory Insights

* 500 store-product inventory records were assessed.
* 393 records were classified as healthy stock.
* 107 records were classified as overstock.
* No records fell below their defined reorder levels.
* Coffee Maker and Vacuum Cleaner were classified as overstock at all 10 stores.

The overstock classification indicates that recorded current stock exceeded the defined maximum stock level. It does not, by itself, prove that products are slow-moving or that excess stock is financially harmful.

## 5. Data Quality and Cleaning

The cleaning workflow addressed:

* Missing and zero quantities
* Duplicate order IDs
* Inconsistent or incorrect payment-method values
* Invalid store, product, and customer references
* Invalid order dates and dates outside the reporting period
* Incorrect sales, cost, and profit calculations
* Invalid discounts and unit prices

Validation checks were used to confirm that the cleaned transaction dataset contained 1,000 records and that the tested data-quality conditions were resolved.

## 6. Business Recommendations

### Recommendation 1: Review Inventory Thresholds

Investigate why Coffee Maker and Vacuum Cleaner records exceeded maximum stock levels across all stores. Validate their reorder levels, maximum stock settings, and actual demand before adjusting purchasing plans.

### Recommendation 2: Improve Inventory Reporting

Connect inventory movements to transaction-level sales so that units sold, closing stock, and replenishment needs can be reconciled consistently.

### Recommendation 3: Monitor Store Performance Using Multiple KPIs

Compare revenue, profit, and profit margin together instead of ranking stores solely by sales. In a real retail environment, this would support a more balanced performance review.

### Recommendation 4: Establish Routine Data Quality Checks

Run validation checks for duplicate IDs, missing quantities, invalid references, date ranges, discounts, and calculated financial amounts before publishing reports.

## 7. Tools and Skills Demonstrated

* Microsoft Excel for data cleaning, formulas, validation, aggregation, and KPI analysis
* SQL learning and analytical thinking
* Business requirements and KPI documentation
* Data dictionaries and data-quality documentation
* Business insight development and recommendation writing
* GitHub project documentation

## 8. Limitations

This project uses synthetic data. Store and product assignments follow repeating patterns, and inventory units sold were generated separately from transaction-level sales. Consequently, observed differences are illustrative rather than evidence of real operational performance.

A production-ready analysis would connect inventory movements to actual transactions, validate business rules with stakeholders, and incorporate purchase orders, returns, stock adjustments, and historical demand.

## 9. Conclusion

This project demonstrates an end-to-end analytical workflow: defining a business problem, documenting requirements, cleaning and validating data, calculating KPIs, comparing sales performance, evaluating inventory status, and translating results into business recommendations.
