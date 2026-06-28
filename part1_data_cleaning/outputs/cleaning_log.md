# Cleaning Log – Part 1: Data Cleaning

## Dataset
raw_orders.xlsx

---

## Issues Found

- Missing values in Region.
- Missing values in Ship Mode.
- Missing Discount values.
- Potential duplicate Order IDs.
- Potential exact duplicate records.
- Invalid shipping dates (Ship Date earlier than Order Date).
- Discounts outside the expected range.
- Records requiring data quality review.

---

## Cleaning Actions Performed

- Filled missing Region values with **"Unknown"**.
- Filled missing Ship Mode values with **"Unknown"**.
- Replaced missing Discount values with **0** where appropriate.
- Added calculated fields using Excel formulas:
  - Calculated Sales
  - Calculated Profit
  - Profit Margin
  - Shipping Delay (Days)
  - Order Month
  - Order Year
  - Data Quality Flag
- Applied conditional formatting to highlight records requiring review.
- Created quality check summaries.
- Created duplicate and invalid record review sheets.
- Created pivot summaries for business reporting.

---

## Business Rules Applied

- Missing Region → Unknown
- Missing Ship Mode → Unknown
- Missing Discount → 0 (where appropriate)
- Flag negative discounts.
- Flag unusually high discounts.
- Flag Ship Date earlier than Order Date.
- Remove exact duplicate records if present.
- Flag conflicting Order IDs for manual review.
- Exclude Cancelled, Refunded and Failed orders from completed sales reporting.

---

## Assumptions Made

- Unknown values are preferable to blank values for reporting.
- Missing discounts indicate no discount unless other data suggests otherwise.
- Flagged records require business review rather than automatic correction.
- Formula-generated fields should remain dynamic instead of being converted to static values.

---

## Records Removed

- No records were permanently deleted.
- Exact duplicates were identified for review where applicable.

---

## Records Flagged

Records were flagged for:

- Missing Region
- Missing Ship Mode
- Negative Discount
- High Discount
- Invalid Shipping Dates
- Duplicate Order IDs
- Data Quality Issues

---

## Limitations

- Business rules are based solely on the provided assignment instructions.
- Some flagged records require manual business validation.
- Calculated values depend on the accuracy of the original source data.