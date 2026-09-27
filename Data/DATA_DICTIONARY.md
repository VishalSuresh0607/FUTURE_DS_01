# Data Dictionary — SuperStore_Sales_Dataset.csv

| Column | Type | Description |
|---|---|---|
| Order ID | Text | Unique identifier for each order (one order can contain multiple line items) |
| Order Date | Date | Date the order was placed |
| Ship Date | Date | Date the order was shipped |
| Ship Mode | Text | Shipping method: Standard Class, Second Class, First Class, Same Day |
| Customer ID | Text | Unique customer identifier |
| Customer Name | Text | Customer full name |
| Segment | Text | Customer segment: Consumer, Corporate, Home Office |
| Country | Text | Country of sale (United States) |
| City | Text | City of sale |
| State | Text | State of sale |
| Region | Text | Sales region: East, West, Central, South |
| Product ID | Text | Unique product identifier |
| Category | Text | Product category: Furniture, Office Supplies, Technology |
| Sub-Category | Text | Product sub-category (e.g., Chairs, Binders, Phones) |
| Product Name | Text | Full product name |
| Sales | Decimal | Revenue for the line item, in USD |
| Quantity | Integer | Units sold in the line item |
| Profit | Decimal | Profit for the line item, in USD (can be negative) |
| Returns | Binary (0/1) | Whether the line item was returned |
| Payment Mode | Text | Payment method: COD, Cards, Online |
| AvgDelivery | Integer | Calculated column — days between Order Date and Ship Date |

**Row count:** 5,901 line items across 3,003 unique orders and 773 unique customers
**Date range:** January 1, 2019 – December 31, 2020

## Notes on data quality
- `Returns` originally contained `#N/A` for non-returned orders; these were standardized to `0` during the Power Query load step.
- `AvgDelivery` is a calculated (DAX) column, not sourced directly from the raw CSV: `DATEDIFF('SuperStore_Sales_Dataset'[Order Date], 'SuperStore_Sales_Dataset'[Ship Date], DAY)`.
- Two helper/index columns (`ind1`, `ind2`) present in the raw source file were removed during cleaning as they carried no analytical value.
