# Interactive Retail Sales Dashboard (Power BI)

Personal project: an interactive Power BI dashboard that analyzes retail sales performance across stores, regions, products, pricing, and customer behavior.

## Overview

- 25,000+ retail transactions across 100 stores in 5 regions (2023-2026)
- $44.4M+ in total sales and 647K+ units sold
- 7 product categories: Beauty, Clothing, Electronics, Groceries, Home & Kitchen, Sports, Toys
- 4 store types: Convenience Store, Hypermarket, Online Store, Supermarket

The dashboard is built around business questions, and each chart answers one of them:

| Question | Visual |
|---|---|
| Is the business growing year over year? | Total sales and total units by year |
| How much of our sales come from promotions? | Total sales by promotion |
| Which cities sell the most? | Top 5 cities by sales |
| Do holidays and weather affect sales? | Units sold per record by weather and day type |
| Do we sell more when our price is lower than competitors? | Price gap impact on units sold per record |
| Do happier customers return fewer items? | Customer satisfaction and return rate by brand |

## Features

- KPI cards: average discount, average units per record, average sales per record, average customer satisfaction, average supplier rating, and return rate
- Interactive slicers for store type, product category, product type, and demand level
- Advanced DAX measures for the KPIs, price gap groups, and comparisons
- Cross-filtering between visuals, so every chart updates when a slicer is used

## Key Findings

- **Sales are flat across the years.** Total sales moved only between $11.01M and $11.23M per year (2023-2026), and units stayed between 160.8K and 163.2K. The business is stable, not growing quickly.
- **Promotions drive most of the sales.** Sales from promoted items were $31M (69%), compared with $14M (31%) from non-promoted items.
- **Holidays have a big effect.** Average units per record were 37.34 on holidays versus 24.02 on regular days, about 55% higher. Across weather conditions, sunny days had the highest units per record (27.57) and stormy days the lowest (21.81).
- **Price matters.** Units sold per record fall steadily as our price moves above competitors: 31 units when we are 15%+ cheaper, 25 when prices are similar, and 21 when we are 15%+ pricier.
- **Top cities are close together.** Dallas ($4.72M), Chicago ($4.58M), Seattle ($4.57M), Denver ($4.47M), and Houston ($4.43M) are within about 6% of each other, so sales are not concentrated in one city.
- **No clear link between satisfaction and returns by brand.** Brand satisfaction scores are very close (4.08-4.11) and return rates range from about 3.4% to 3.7%, so satisfaction alone does not explain which brands get more returns.

## Files

- `retail-sales-dashboard.pdf`: exported dashboard report, viewable without Power BI
- `retail-sales-dashboard.pbix`: the Power BI file, open it in Power BI Desktop to use the slicers and see the DAX measures

The slicers only work in the `.pbix` file. The PDF shows the dashboard in its default view.

## Data

[Retail Sales Forecast Dataset 2026](https://www.kaggle.com/datasets/mmumairkhattak/retail-sales-forecast-dataset-2026) from Kaggle (25,000 retail sales records). The dataset is tagged as synthetic, so the findings above describe this dataset and not real-world retail performance. It contains no personal or company data.

## Tools

Power BI, DAX, Power Query
