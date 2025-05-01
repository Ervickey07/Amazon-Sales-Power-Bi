#Amazon Analysis Products Sells 

## 📊 Sales Analytics Dashboard - Problem Statements & Chart Requirements

This project aims to analyze and visualize year-to-date (YTD) sales and review data to uncover key business insights using visual storytelling. Below are the primary problem statements and the chart requirements for this dashboard.

---

### ✅ Problem Statements

1. **How do sales trends evolve throughout the year?**
2. **Are there any significant fluctuations in weekly sales performance?**
3. **Which product categories are generating the highest and lowest sales?**
4. **What are the top-performing products contributing most to revenue?**
5. **Which products are most preferred by customers based on reviews?**

---

### 📈 Charts Requirements

1. ### **YTD Sales by Month (Line Chart)**
   - **What:** Visualize the total sales aggregated by each month.
   - **Why:** To identify seasonal trends and understand overall monthly growth patterns.
   - **Chart Type:** Line Chart  
   - **Insight Goal:** Detect sales peaks, dips, and steady growth phases.

2. ### **YTD Sales by Week (Column Chart)**
   - **What:** Break down sales data by individual weeks.
   - **Why:** To highlight short-term fluctuations and weekly performance patterns.
   - **Chart Type:** Column (Bar) Chart  
   - **Insight Goal:** Spot weekly anomalies or high-performing campaigns.

3. ### **Sales by Product Category (Text or Heat Map)**
   - **What:** Show total sales grouped by product category.
   - **Why:** To compare and assess category-wise performance visually.
   - **Chart Type:** Heat Map or Text Summary  
   - **Insight Goal:** Quickly identify top-performing and underperforming product categories.

4. ### **Top 5 Products by YTD Sales (Bar Chart)**
   - **What:** Display the top 5 individual products based on total YTD sales.
   - **Why:** To spotlight the best-selling products and their contribution to revenue.
   - **Chart Type:** Bar Chart (Vertical/Horizontal)  
   - **Insight Goal:** Focus decision-making on high-impact products.

5. ### **Top 5 Products by YTD Reviews (Bar Chart)**
   - **What:** Identify the 5 most-reviewed products year-to-date.
   - **Why:** To understand customer preferences and product popularity based on review count.
   - **Chart Type:** Bar Chart  
   - **Insight Goal:** Highlight customer-favorite products and gather qualitative insight for marketing or inventory strategies.

---

### 🧠 Power BI Features Used

#### 🧩 DAX Functions
- `CONCATENATE` – Combined product names and categories for better context
- `FORMAT` – Applied to dates and numbers for user-friendly display (e.g., `FORMAT([Sales], "$#,##0")`)
- `DATE`, `YEAR`, `MONTH` – Extracted and created date-based columns for slicing/filtering
- `CALCULATE`, `FILTER`, `ALL` – Built dynamic YTD sales measures

#### 🧮 Custom Measures & Calculated Columns
- YTD Total Sales
- Review Counts by Product
- Monthly and Weekly Sales Growth

#### 🧾 New Tables Created
- **Date Table**: Custom date table using `CALENDAR()` for accurate time intelligence  
- **Top 5 Product Tables**: Used `TOPN()` in combination with `SUMMARIZE` to rank products by sales and reviews

#### 🔗 Data Modeling
- Established **many-to-one relationships** between:
  - Product Table ↔ Sales Table  
  - Date Table ↔ Sales Table  
  - Category Table ↔ Product Table  
- Ensured **bi-directional filtering** where needed for drill-through analysis

---

### 🛠️ Tools & Stack

- **Power BI** – Data visualization and modeling  
- **DAX** – Custom logic and calculated measures  
- **Power Query** – Data transformation and cleaning  
- **SQL & Python** – (Used as external preprocessing options)

---

### 💡 Insights Gained

- Identified **seasonal sales peaks** and weekly fluctuations  
- Found top-selling categories and **underperformers** for action planning  
- Pinpointed **customer-favorite products** by review volume  
- Created an interactive model ready for **executive-level storytelling**

---

### 👨‍🏫 Guided By
**Mentor:** *Divakr Kushwaha Sir* – Thank you for your continued support and mentorship throughout this journey.


📂 **Data Source:** *(e.g., Internal CRM & Review Database, Kaggle Retail Dataset)*  
🛠️ **Tools Used:** Power BI | Python | SQL *(Modify as needed)*  
📅 **Time Frame:** Year-To-Date (YTD)

---






