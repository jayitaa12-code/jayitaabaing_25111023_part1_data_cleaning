# Business Analytics Assignment – Part 1: Data Cleaning

## Problem Summary

The objective of this assignment is to improve the quality of a raw sales dataset by identifying and correcting data quality issues while preserving the original data. The cleaned dataset is then used to generate business summaries and insights.

---

## Dataset Description

Dataset: **raw_orders.xlsx**

The dataset contains order-level sales transactions including:

- Order information
- Customer details
- Product details
- Sales
- Profit
- Discount
- Region
- Ship Mode
- Shipping Dates

---

## Tools Used

- Microsoft Excel
- Excel Formulas
- Pivot Tables
- Conditional Formatting

---

## Cleaning Steps Performed

- Reviewed the dataset against the provided business rules.
- Filled missing Region values with **Unknown**.
- Filled missing Ship Mode values with **Unknown**.
- Filled missing Discount values with **0** where applicable.
- Created calculated fields using Excel formulas.
- Identified duplicate records.
- Flagged conflicting Order IDs.
- Flagged invalid shipping dates.
- Applied conditional formatting to highlight issues.
- Generated quality summaries.
- Generated pivot reports.

---

## Business Rules Applied

- Missing Region → Unknown
- Missing Ship Mode → Unknown
- Missing Discount → 0
- Flag negative discounts.
- Flag high discounts.
- Flag Ship Date earlier than Order Date.
- Remove exact duplicates where applicable.
- Flag conflicting Order IDs.
- Exclude Cancelled, Failed and Refunded orders from completed sales summaries.

---

## Summary of Data Quality Issues Found

The following issues were identified during cleaning:

- Missing Region values
- Missing Ship Mode values
- Missing Discount values
- Duplicate Order IDs
- Invalid Shipping Dates
- High Discounts
- Negative Discounts

Records requiring manual review were flagged rather than automatically modified.

---

## Summary of Pivot Reports

The workbook includes summaries for:

- Sales by Region
- Sales by Category
- Profit by Region
- Monthly Sales
- Average Shipping Delay

These summaries provide a high-level overview of sales performance and operational trends.

---

## Key Business Insights

- Sales performance varies across regions.
- Certain product categories generate higher profits than others.
- Shipping performance differs by order.
- Data quality issues can significantly affect business reporting.
- Cleaning and validation improve reporting accuracy and consistency.

---

## Assumptions

- Blank Region and Ship Mode values are treated as Unknown.
- Blank Discount values represent no discount unless business logic indicates otherwise.
- Flagged records require manual review instead of automatic correction.
- Formula-based calculations remain dynamic.

---

## Limitations

- Analysis depends on the quality of the source data.
- Business rules were limited to those provided in the assignment.
- Flagged records may require additional investigation outside the scope of this assignment.

---

## Screenshots Included

The repository contains screenshots showing:

- Original dataset
- Formula columns
- Conditional formatting
- Quality checks
- Duplicate review
- Invalid records
- Pivot summaries
- Final workbook structure