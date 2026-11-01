# 📊 ShopKart India E-Commerce Sales & Profitability Analysis Dashboard

## 📌 Executive Summary
The **ShopKart India E-Commerce Dashboard** is an end-to-end data analysis and business intelligence project built using Microsoft Excel. This interactive dashboard evaluates transactional data containing **2,500 orders** across multiple product categories, geographic regions (Indian States), sales channels, and order statuses.

The primary objective of this project is to model, analyze, and visualize core e-commerce metrics—such as Net Sales, Profitability, Average Order Value (AOV), Profit Margins, and Fulfillment Efficiency—enabling stakeholders to optimize inventory, marketing strategies, and regional delivery operations.

---

## 🔑 Key Performance Indicators (KPIs)
Based on the synthesized dataset, the dashboard highlights the following high-level business metrics:

| Metric | Value | Description |
| :--- | :--- | :--- |
| **Total Orders** | `2,500` | Total number of customer transactions logged in the system. |
| **Total Quantity Sold** | `2,163` units | Aggregated quantity of items purchased across all categories. |
| **Total Net Sales** | `₹ 63,50,229.95` | Total revenue generated after discounts. |
| **Total Profit** | `₹ 19,20,523.95` | Cumulative net profit earned from sales. |
| **Average Order Value (AOV)** | `₹ 2,540.09` | Average monetary revenue generated per order. |
| **Overall Profit Margin** | `30.24%` | Overall profitability percentage across all transactions. |

---

## 📁 Dataset Schema & Field Descriptions
The underlying dataset consists of **2,500 rows** structured with the following fields:

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `Month Of Order` | Date/Text | The month in which the order was placed (Jan – Dec). |
| `State` | Text | Geographic destination state in India (e.g., UP, Kerala, Maharashtra). |
| `Gender` | Text | Demographics of the customer (Female / Male). |
| `Product_Category` | Text | Category of item purchased (Electronics, Fashion, Sports, etc.). |
| `Payment_Mode` | Text | Payment method used (Credit Card, Debit Card, UPI, Net Banking, COD). |
| `Sales_Channel` | Text | Channel through which the sale occurred (Amazon, Flipkart, Mobile App, Website). |
| `Order_Status` | Text | Current status of the order (Delivered, Cancelled, Returned). |
| `Delivery_Days` | Integer | Duration taken (in days) to complete delivery. |
| `Cost_Per_Unit` | Currency (INR) | Wholesale / Acquisition cost per unit. |
| `Discount Amount` | Currency (INR) | Total discount granted on the order. |
| `Gross Sales` | Currency (INR) | Revenue generated before applying discounts. |
| `Net Sales` | Currency (INR) | Final revenue generated after discount subtraction (`Gross Sales - Discount Amount`). |
| `Total Cost` | Currency (INR) | Total expense incurred for the order (`Cost Per Unit × Quantity`). |
| `Profit` | Currency (INR) | Net monetary gain (`Net Sales - Total Cost`). |
| `Profit Margin %` | Percentage | Profitability relative to sales (`(Profit / Net Sales) × 100`). |
| `Profit Status` | Text | Indicator flag evaluating order profitability (e.g., High Profit, Low Profit, Loss). |

---

## 📈 Dashboard Visualizations & Insights

### 1. Monthly Sales & Profitability Trends
* **Monthly Sales Analysis (Column Chart):** Tracks revenue stability across the year (Jan – Dec), showing consistent volume between ₹4.5L and ₹6.0L per month.
* **Monthly Net Sales vs. Profit Analysis (Combo Line & Bar Chart):** Evaluates relationship trends between total revenue and realized net profit across monthly timeframes.

### 2. Category Performance Analysis
* **Profit by Product Category (Horizontal Bar Chart):**
  * 🏆 **Top Performers:** *Electronics* (~₹5.5L profit) and *Fashion* (~₹4.8L profit) drive the majority of profits.
  * 📦 **Moderate Performers:** *Home & Kitchen* (~₹3.9L profit) and *Sports* (~₹2.8L profit).
  * ⚠️ **Lowest Performers:** *Beauty* (~₹1.1L profit) and *Grocery* (~₹70K profit).

### 3. Geographic Sales Distribution
* **Top 10 States by Net Sales (Horizontal Bar Chart):**
  * **Leading Market:** *Uttar Pradesh* leads in net sales, followed closely by *Kerala*, *Bihar*, and *Maharashtra*.
  * **Secondary Markets:** *West Bengal*, *Tamil Nadu*, *Delhi*, *Gujarat*, *Odisha*, and *Karnataka*.

### 4. Fulfillment & Order Health
* **Order Status Breakdown (Donut Chart):**
  * ✅ **Delivered:** `87%` (Successful operational delivery rate).
  * ❌ **Cancelled:** `7%` (Lost revenue due to pre-fulfillment cancellations).
  * 🔄 **Returned:** `6%` (Post-fulfillment return rate requiring reverse logistics).

---

## 🎛 Interactivity & Filtering (Slicers)
The dashboard features dynamic **Excel Slicers** allowing multi-dimensional data drilling:
1. **Month Of Order:** Filter by specific months or quarters.
2. **State:** Drill down into specific Indian states/territories.
3. **Gender:** Segment purchasing behavior between Male and Female shoppers.
4. **Product Category:** Isolate metrics for specific product lines (Beauty, Electronics, Fashion, Grocery, Home & Kitchen, Sports).
5. **Order Status:** Filter by Delivered, Cancelled, or Returned orders.
6. **Sales Channel:** Compare channel performance across Amazon, Flipkart, Mobile App, and Website.

---

## 🛠 Tech Stack & Tools Used
* **Software:** Microsoft Excel (Office 365 / Excel 2019+)
* **Data Transformation:** Power Query / Excel Formulas (`SUMIFS`, `AVERAGEIFS`, `VLOOKUP`, `CALCULATE`)
* **Data Modeling:** Power Pivot & Data Model Setup
* **Visualization:** Custom Pivot Charts, Pivot Tables, Formatted KPIs, Dynamic Slicers
* **UI/UX Design:** Dark Theme Header Banner with Color-Coded Metric Cards (Green = Sales, Orange = Profit, Red = Margin)

---

## 💡 Business Recommendations
1. **Capitalize on Core Categories:** Reallocate marketing budget toward **Electronics** and **Fashion**, which yield significantly higher profit margins than Grocery and Beauty.
2. **Optimize Channels & Logistics in Top States:** Streamline delivery networks in high-volume states (**Uttar Pradesh**, **Kerala**, **Bihar**, and **Maharashtra**) to maintain high customer satisfaction.
3. **Reduce Return & Cancellation Rates:** Investigate reasons behind the **13% combined non-delivery rate** (7% cancelled + 6% returned) to recover revenue loss and lower reverse logistics costs.

---

## 🚀 How to Run the Project
1. Download or clone this repository.
2. Open `ShopKart_India_Ecommerce_Dashboard.xlsx` in Microsoft Excel (version 2016 or newer recommended).
3. Ensure macros/content are enabled if prompted.
4. Interact with the **Slicers** on the left menu to slice and dice the metrics dynamically.