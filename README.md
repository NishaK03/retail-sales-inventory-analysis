# NovaMart Retail — Sales & Inventory Performance Analysis

An end-to-end Business Analyst portfolio project demonstrating data cleaning, data quality validation, KPI development, retail sales analysis, inventory monitoring, and business recommendations using synthetic retail data.

## Project Overview

NovaMart Retail is a fictional multi-store retailer created to demonstrate how business analysts can turn raw operational data into structured insights for business decision-making.

This project examines simulated 2026 sales transactions and a year-end inventory snapshot to explore sales performance, product contribution, store-level profitability, and inventory status.

## Business Questions

* What are the overall sales, profit, and profit margin?
* Which products generate the highest revenue?
* How do sales and profitability vary across stores?
* How many store-product combinations are classified as low stock, healthy stock, or overstock?
* What data quality issues should be resolved before business reporting?
* What actions could help improve reporting reliability and inventory monitoring?

## Tools & Skills

* **Excel:** data cleaning, formulas, conditional logic, aggregations, validation, and KPI calculations
* **Business Analysis:** business problem definition, requirements documentation, KPI definitions, and recommendations
* **Data Quality:** duplicate checks, missing-value checks, reference validation, date validation, and financial calculation checks
* **GitHub:** project organization and documentation

## Dataset Overview

| Dataset   | Records | Purpose                                           |
| --------- | ------: | ------------------------------------------------- |
| Orders    |   1,000 | Transaction-level sales and profit analysis       |
| Products  |      50 | Product attributes, pricing, and stock thresholds |
| Stores    |      10 | Store-level performance analysis                  |
| Customers |     300 | Customer reference data                           |
| Inventory |     500 | Year-end stock status by store and product        |

All data is synthetic and was created for portfolio demonstration. It does not represent a real retailer.

## Key Results

| KPI                 |     Result |
| ------------------- | ---------: |
| Total Sales         | ₹45,08,300 |
| Total Profit        | ₹17,83,900 |
| Profit Margin       |     39.57% |
| Average Order Value |  ₹4,508.30 |
| Units Sold          |      3,000 |
| Transactions        |      1,000 |
| Inventory Records   |        500 |
| Low-Stock Records   |          0 |
| Overstock Records   |        107 |
| Overstock Rate      |     21.40% |

## Key Insights

### Sales Performance

* **Highest-sales store:** NovaMart Lucknow Central, with ₹9,31,600 in sales.
* **Highest-profit store:** NovaMart Lucknow Central, with ₹3,31,600 in profit.
* **Highest-revenue product:** Vacuum Cleaner, with ₹5,19,920 in sales.
* Air Fryer and Food Processor were the next two highest-revenue products in the simulated dataset.

### Inventory Monitoring

* 107 of 500 store-product records were classified as overstock.
* No records were below their defined reorder levels.
* Coffee Maker and Vacuum Cleaner were classified as overstock at all 10 stores.

These are descriptive results from simulated data. They should not be interpreted as evidence of actual retail demand or operational performance.

## Data Cleaning & Validation

The workflow addressed missing and zero quantities, duplicate order IDs, inconsistent payment-method values, invalid reference IDs, date issues, discount values, unit prices, and sales, cost, and profit calculations.

Quality checks were used to validate the cleaned transaction dataset and verify key business rules.

## Business Recommendations

1. **Review inventory thresholds:** Investigate products repeatedly exceeding maximum stock levels before changing replenishment policies.
2. **Integrate inventory and sales data:** Derive units sold from transaction records and reconcile stock movements with closing inventory.
3. **Monitor multiple store KPIs:** Evaluate revenue, profit, and profit margin together rather than relying on sales alone.
4. **Standardize data quality checks:** Validate transactions before using them in recurring reports and management dashboards.

## Project Structure

```text
retail-sales-inventory-analysis/
├── README.md
├── workbook/
│   └── NovaMart_Retail_Analysis.xlsx
├── documentation/
│   ├── business_problem.md
│   ├── business_requirements.md
│   ├── KPI_definitions.md
│   ├── data_dictionary.md
│   └── business_insights.md
└── analysis/
    └── data_cleaning.md
```


## Limitations

The datasets are synthetic, and the generated store-product assignments follow repeating patterns. Inventory units sold were generated separately from transaction-level orders. Therefore, store comparisons and inventory findings are illustrative rather than evidence of real operational performance.

A production-ready analysis would reconcile inventory movements with transaction data and incorporate purchase orders, returns, stock adjustments, and historical demand.

## Conclusion

This project demonstrates a structured Business Analyst workflow: defining business questions, documenting requirements, cleaning data, validating business rules, calculating KPIs, comparing performance, and translating findings into actionable recommendations.
