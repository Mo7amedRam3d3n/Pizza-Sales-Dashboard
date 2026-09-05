# Pizza Sales Dashboard – Excel Pivot Table Analysis
An end-to-end sales analysis project built entirely in Microsoft Excel, using **Pivot Tables**, **Pivot Charts**, and an **interactive Dashboard** to explore pizza sales performance across categories, sizes, and time.
---
##  Project Overview
This project analyzes a full year of pizza sales transactions to answer key business questions such as:
- Which pizza category and size sell the most?
- How do sales change month over month?
- What is the total revenue, quantity sold, and customer count?
- What is the revenue split before and after tax?
The final output is a single-page, interactive Excel dashboard connected to slicers for `pizza_category` and `pizza_size`.
---
##  Dataset
The raw dataset contains individual pizza order records with the following fields:
Column	Description
order_id	Unique ID for each order
pizza_id	Unique ID for each pizza variant (size + type)
Customer Name	Name of the customer who placed the order
quantity	Number of pizzas ordered
order_date	Date when the order was placed
order_time	Time when the order was placed
unit_price	Price of one pizza
total_price	Total price of the order (quantity × unit_price)
pizza_size	Pizza size: S, M, L, or XL
pizza_category	Pizza category: Classic, Chicken, Supreme, or Veggie
pizza_ingredients	List of ingredients used in the pizza
pizza_name	Full descriptive name of the pizza

---
## Tools Used
- **Microsoft Excel**
  - Pivot Tables & Pivot Charts
  - Slicers (for interactivity)
  - Powe Query
  - Calculated fields (tax and after-tax price)
---
##  Steps Taken
1. Data Cleaning and Preparation
- Converted the order_time column from Numeric Data Type to a proper Time format.
- Ensured consistency in values within the Pizza Category and Pizza Size columns.
- Verified the data types and formatting of the columns to ensure accurate analysis.
- Checked for obvious errors or inconsistent values that could affect the analysis results.

2. Building Pivot Tables
Multiple pivot tables were created to break down the data from different angles:
- **Quantity by Category** — total pizzas sold per category (Classic, Veggie, Supreme, Chicken)
- **Quantity by Size** — total pizzas sold per size (S, M, L, XL)
- **Total Price by Category & Size** — revenue breakdown
- **Monthly Sales** — total revenue and quantity sold per month (Jan to Dec)
- **Percent of Category** — each category's share of total quantity sold
- **Tax Summary** — total price, 14% tax, and price after tax per category
- **Summary KPIs** — Total Customers, Total Sales, Total Quantity Sold

3. Building the Dashboard
Using the pivot tables above, an interactive one-page dashboard was designed with:
- **KPI Cards**: Total Customers, Total Sales, Total Quantity Sold
- **Bar Chart**: Quantity by Category
- **Bar Chart**: Quantity by Size
- **Pie Chart**: Percent of Category
- **Line Chart**: Monthly Sales trend
- **Slicers**: to filter by “pizza_category” and “pizza_size”
- A link/button to navigate to the source pivot tables
---
## Key Insights
- **Total Sales:** $8,436 | **Total Quantity Sold:** 511 pizzas | **Total Customers:** 499

- **Classic** is the best-selling category (152 pizzas, ~29.75% of sales), followed by **Veggie** (141, ~27.59%), **Supreme** (122, ~23.87%), and **Chicken** (96, ~18.79%).

- **Large (L)** is by far the most popular size (202 pizzas sold), while **XL** is the least ordered (only 11).

- Monthly sales show a clear seasonal pattern, peaking between **May and August** (highest in May at $832) and dipping in **February** ($528) and **November** ($597).

- After applying a 14% tax, total revenue increases from $8,436.05 to approximately **$9,617.10**.
---

##  How to Use
1. Download `pizza_sales_dashboard.xlsx`
2. Open it in Excel (2016 or later recommended for full slicer support)
3. Use the slicers on the dashboard to filter by category or size
4. Click the "View Source" button to explore the underlying pivot tables
---
##  Author
Built by [Mohamed Ramadan] as a data analysis portfolio project.
