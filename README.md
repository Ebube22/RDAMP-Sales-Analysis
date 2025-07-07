# RDAMP-Sales-Analysis

## Project Overview

This project is an initial business intelligence report for a Super store named Ace which is a nationwide retail chain that is currently experiencing rapid growth. The report generated is based on a detailed analysis of the company's historical sales data which is targeted at providing actionable insights that suggests regional expansion and optimization of opreations.

**Objectives**: The main Objective is to deliver key insights on sales performance trends, opportunities in regional growth, customer behavior patterns, and product-level profitability.

The business questions addressed are:
- Regional and segment sales and discount performance
- Product-level profits and margin analysis
- Location-based completeness and data consistency
- Top and Underperforming Product Identification

##Tools Used
- Python(Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Excel for initial Data Exploration
- GitHub for Portfolio Hosting

--- 
## Tasks Completed ✅

###1. Data Quality Assessment

- I checked for and addressed **duplicates** and found none.
- I identified and flagged:
  - **197 rows** with anomalous discounts
  - **0** with invalid quantity
  - **42 rows** with invalid costs
- I verified that no missing critical values were dropped unnecessarily
- I identified missing or null values for Country, Category, Region, and mapped them to fill up the missing data

---

### 2. Sales, Revenue, and Discount Rates by Region and Segment
- I created a **Segment** column by splitting the 'Category' column
- I grouped the data by **Region** and **Segment**to compute the total **Sales** and Average **Discount** per grouping

**Insights**: Scotland has the highest total sales, followed by East Midlands and London, while Wales has the lowest Total Sales

---

### 3. Best and Underperforming Products by Revenue

### Top 5 Best-Selling Products by Revenue 


|Product Name                   |Sales |        |Quantity |   |Discount    |
|Portable Refrigerator Freezer  |4504.38 |      |171      |   |0.150000    |
|Electric Bike                  |4499.25 |      |53       |   |0.214000    |
|Portable Solar Generator       |3998.20 |      |128      |   |0.206129    |
|Digital Camera                 |3902.86 |      |107      |   |0.086923    |
|Compact Digital Camera         |2998.17 |      |133      |   |0.135000    |


 **Bottom 5 Underperforming Products by Revenue**

|Product Name          |Sales |   |Quantity   |   |Discount  |
|Canned Black Beans    |1.29  |   |7          |   |0.270000  |
|Flavored Rice Cakes   |1.49  |   |12         |   |0.080000  |
|Tomato Paste          |1.87  |   |29         |   |0.136667  |
|Sesame Seeds          |1.99  |   |20         |   |0.330000  |
|Baking Soda           |2.13  |   |23         |   |0.140000  |

---

### 4. Product Categories with Highest Margins

When computing the highest margin, I noticed Total_Margin was negative for all categories, which means the business might have sold at a loss, or the cost price of the data is off

The product with the highest Margin is **Food - Dressing**

**Output:** 
Top Category by Total Margin:
Category          Food - Dressing
Total_Margin               -3.571
Average_Margin          -1.190333
Total_Sales                  7.17

---

### 5. Sales Distribution: Online vs In-store
- This was grouped by the 'Order Mode' and visualized sales by pie chart

**Result**:
**Online Sales**: 51.6%
**In-store Sales**: 48.4%

---

## Visualizations

1. **Bar Plot**: Total Sales by Region
   Insight: East Midlands leads with Total Sales by Region
2. **Pie Chart**: Sales Distribution-Online vs In-Store
   Insight: Most products were sold online.
3. **Bar Charts**:
   - Top 5 Best-Selling Products
   - Bottom 5 Underperforming Products

## Recommendations
- The company should review pricing strategies
- There should be target promotions in high-performing segments
- Clean mapping inconsistencies 
- All low-revenue generating products should phase out since they don't add value
- There should be an investment in best sellers.

-----

# Project Structure
