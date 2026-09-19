# Superstore Sales Dashboard

Power BI dashboard for exploring Superstore sales, profit, customers, products, shipping, and short term sales trends.

## Project Contents

| File | Description |
| --- | --- |
| [SuperStore_Sales_Dashboard.pbix](SuperStore_Sales_Dashboard.pbix) | Editable Power BI report |
| [SuperStore_Sales_Dashboard.pdf](SuperStore_Sales_Dashboard.pdf) | Exported report for sharing or printing |
| [SUperstore Sales Dashboard.png](SUperstore%20Sales%20Dashboard.png) | Sales analysis dashboard preview |
| [Forecast Dashboard.png](Forecast%20Dashboard.png) | Forecast dashboard preview |
| [Dataset/SuperStore_Sales_Dataset.csv](Dataset/SuperStore_Sales_Dataset.csv) | Source transaction data |

## Dashboard Pages

### Superstore Sales Analysis

- KPI cards for sales, quantity, profit, and average delivery
- Sales by customer segment and region
- Profit by year and sales by year
- Sales by ship mode, category, and sub-category
- Geographic view of profit by state and sales
- Region slicer for Central, East, South, and West

### Sales Forecast

- Sales by order date across 2019 and 2020
- 15-day sales forecast view
- Sales by state, with the highest-sales states highlighted

## Dataset

The CSV contains 5,901 transaction rows and 23 columns. Order dates cover January 1, 2019 through December 31, 2020. The data represents United States orders and includes:

- Order and shipment details: `Order ID`, `Order Date`, `Ship Date`, and `Ship Mode`
- Customer and location details: customer, segment, city, state, and region
- Product details: product ID, category, sub-category, and product name
- Measures: `Sales`, `Quantity`, `Profit`, and `Returns`
- Payment details: `Payment Mode`

The dataset is distributed across the four regions as follows: West (1,901 rows), East (1,688), Central (1,381), and South (931).

## Getting Started

1. Open [SuperStore_Sales_Dashboard.pbix](SuperStore_Sales_Dashboard.pbix) in Power BI Desktop.
2. If Power BI prompts for the source, select [Dataset/SuperStore_Sales_Dataset.csv](Dataset/SuperStore_Sales_Dataset.csv).
3. Refresh the report after changing the source data.
4. Use the region slicer and chart selections to filter the report interactively.

## Data Preparation Notes

- Dates are stored in `dd-MM-yyyy` format in the CSV and may need locale-aware parsing when the source is reconnected.
- `Returns` contains `#N/A` values in the supplied source and should be cleaned or handled explicitly before using it in calculations.
- `ind1` and `ind2` are present in the source header but are blank in the supplied records.

## Output
<img width="1230" height="706" alt="SUperstore Sales Dashboard" src="https://github.com/user-attachments/assets/8323c97b-ce46-4759-82c9-c6b482d442aa" />
<img width="1230" height="703" alt="Forecast Dashboard" src="https://github.com/user-attachments/assets/96788a60-9e6c-4e41-aea4-b006cef9d34c" />
