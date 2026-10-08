# Business Requirements

## Objective

The objective of this project is to analyze NovaMart Retail's sales and inventory data and provide actionable insights that support better business decision-making.

## Functional Requirements

The analysis should allow management to:

1. View overall sales performance.
2. Monitor total revenue and profit.
3. Analyze sales trends over time.
4. Compare performance across stores.
5. Compare performance across product categories.
6. Identify top-performing products.
7. Identify underperforming products.
8. Analyze inventory levels.
9. Identify products with potential stockout risk.
10. Identify products with excess inventory.
11. Understand the relationship between sales performance and inventory levels.
12. View key business metrics through an interactive dashboard.

## Reporting Requirements

The final dashboard should include:

- Total Revenue
- Total Profit
- Total Orders
- Units Sold
- Average Order Value
- Inventory Value
- Low-Stock Products

The dashboard should provide visual analysis of:

- Monthly sales trends
- Store performance
- Category performance
- Product performance
- Inventory health

## Business Rules

### Low Stock

A product is considered at potential stockout risk when:

Current Stock < Reorder Level

### Healthy Stock

A product is considered adequately stocked when:

Current Stock >= Reorder Level

AND

Current Stock <= Maximum Stock Level

### Overstock

A product is considered overstocked when:

Current Stock > Maximum Stock Level
