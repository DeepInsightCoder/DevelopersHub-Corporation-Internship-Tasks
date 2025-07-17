## Interactive Business Dashboard in Streamlit

### Objective

Develop an **interactive business intelligence dashboard** using **Streamlit** to visualize and analyze performance metrics like sales, profit, and customer behavior across regions and product categories.

### Dataset

**Global Superstore Dataset**
Key columns:

* `Region`, `Category`, `Sub-Category`, `Sales`, `Profit`, `Customer.Name`, `Segment`, `Order.Date`, `Ship.Mode`, `Shipping.Cost`

### Features Implemented

1. **Data Cleaning & Preparation**

   * Parsed and converted date columns (`Order.Date`, `Ship.Date`)
   * Removed missing or duplicate entries
   * Extracted time-based features (Year, Month, Week)

2. **Interactive Filters in Sidebar**

   * Region selection
   * Category and Sub-Category dropdowns
   * Date range selector for dynamic analysis

3. **Key Performance Indicators (KPIs)**

   * 📈 Total Sales
   * 💰 Total Profit
   * 👥 Top 5 Customers by Sales
   * Visual KPI indicators with **highlighted metrics**

4. **Visualizations with Streamlit & Plotly**

   * **Bar charts**: Profit by Category & Sub-Category
   * **Line charts**: Sales over time
   * **Pie charts**: Segment-wise contribution
   * **Dynamic tables**: Filtered sales and profit data

5. **User Experience**

   * Responsive design using Streamlit’s layout system
   * Easy-to-use interface for business users
   * Real-time interactivity on filter change


### Skills Gained

* Dashboard development with **Streamlit**
* Business storytelling using **interactive charts**
* Data filtering and **real-time analytics**
* KPI tracking and performance visualization


**Final Output:** A **fully interactive dashboard** that allows business stakeholders to explore performance trends, segment analysis, and high-value customers in a visually engaging way.
