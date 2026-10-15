# Data Cleaning and Quality Assessment

## 1. Purpose

This document describes the data-quality issues intentionally introduced into the raw orders dataset for the NovaMart Retail Sales and Inventory Performance Analysis project.

The purpose is to demonstrate a structured data-cleaning workflow, validate business rules, and prepare reliable data for downstream analysis.

## 2. Data Source

* **Source dataset:** Orders
* **Working copy:** Orders_Raw
* **Original dataset:** Orders
* **Tool:** Google Sheets
* **Expected transaction count before introducing a duplicate:** 1,000 orders

The original Orders sheet is preserved. Data-quality issues are introduced only in the Orders_Raw working copy.

## 3. Identified Data-Quality Issues

### Issue 1: Missing Quantity

* **Location:** Cell F10
* **Column:** Quantity
* **Problem:** The quantity value is missing.
* **Business impact:** Missing quantities can prevent reliable calculation of sales, cost, and profit.
* **Planned action:** Investigate the source record and determine an appropriate correction before using the record in analysis.

### Issue 2: Inconsistent Payment Method

* **Location:** Cell L15
* **Column:** Payment_Method
* **Problem:** The value `upi` uses inconsistent capitalization.
* **Business impact:** Inconsistent labels can split the same payment method into multiple categories during analysis.
* **Planned action:** Standardize the label to `UPI`.

### Issue 3: Duplicate Transaction

* **Location:** Duplicate record containing Order_ID O00019
* **Problem:** The same transaction appears twice in the raw dataset.
* **Business impact:** Duplicate transactions can inflate order counts, revenue, costs, and profit.
* **Planned action:** Compare the records and remove the duplicate only after confirming that it is an unintended duplicate.

### Issue 4: Invalid Quantity

* **Location:** Cell F25
* **Column:** Quantity
* **Problem:** The quantity is recorded as 0.
* **Business rule:** Quantity must be at least 1 for a valid order line.
* **Business impact:** A zero quantity can distort transaction metrics and indicate invalid data.
* **Planned action:** Investigate the record and correct or exclude it based on the available evidence and documented business rules.

## 4. Data-Cleaning Principles

* Preserve the original source data.
* Keep raw and cleaned datasets separate.
* Validate records against defined business rules.
* Investigate questionable values instead of making unsupported assumptions.
* Document each correction and its business justification.
* Recheck the cleaned dataset before analysis.

## 5. Status

The issues listed above have been introduced for demonstration purposes. Cleaning and validation are pending.
