# professional-Data-Analyst-portfolio-project


# ⛽ Petrol Pump Sales Analytics Dashboard

## 📊 Project Overview

This project analyzes **petrol pump sales data for 2025** to understand revenue trends, fuel demand, employee performance, and customer payment behavior.

An interactive dashboard was built using **Power BI** to help stakeholders monitor key business metrics and make informed operational decisions.

The dashboard provides insights into:

* Total revenue and fuel sales
* Pump performance
* Employee sales contribution
* Customer payment preferences
* Shift-wise sales distribution
* Fuel type demand patterns

---

# 🎯 Business Problem

Fuel retail businesses handle thousands of transactions daily. Without proper analytics, it becomes difficult to identify:

* Which petrol pumps generate the highest revenue
* Which employees contribute the most sales
* Which payment methods customers prefer
* When the highest fuel demand occurs

This project aims to solve these problems by building a **visual analytics dashboard** for monitoring operational performance.

---

# 📁 Dataset Description

The dataset contains **fuel sales transaction records** with the following attributes:

| Column            | Description                      |
| ----------------- | -------------------------------- |
| Date              | Transaction date                 |
| Petrol Pump       | Pump name                        |
| Location          | Sales location                   |
| Fuel Type         | Petrol / Diesel / Premium Petrol |
| Quantity (Liters) | Fuel sold in liters              |
| Price per Liter   | Fuel price                       |
| Total Sales       | Total revenue per transaction    |
| Payment Mode      | Cash / Card / UPI                |
| Employee          | Staff handling the transaction   |
| Shift             | Morning / Evening / Night        |

---

# 🧹 Data Cleaning & Preparation

Data transformation was performed using **Power Query**.

Steps included:

* Verified and corrected **data types**
* Created **Year and Month columns**
* Checked for missing values
* Ensured **consistent payment mode categories**
* Validated total revenue calculations

Example transformation:

```
Month = FORMAT([Date],"MMM")
Year = YEAR([Date])
```

---

# 📈 Key Metrics (DAX Measures)

### Total Revenue

```
Total Revenue = SUM(FuelData[Total Sales])
```

### Total Fuel Sold

```
Total Fuel Sold = SUM(FuelData[Quantity (Liters)])
```

### Total Transactions

```
Total Transactions = COUNTROWS(FuelData)
```

### Average Transaction Value

```
Avg Transaction Value =
DIVIDE([Total Revenue],[Total Transactions])
```

---

# 📊 Dashboard Features

The dashboard includes multiple interactive visualizations:

### KPI Cards

* Total Revenue
* Total Fuel Sold
* Total Transactions
* Average Transaction Value

### Visual Insights

* Revenue trend over time
* Fuel type distribution
* Pump performance comparison
* Employee sales analysis
* Payment method distribution
* Shift-wise sales performance
* Geographic sales distribution

### Interactive Filters

Users can filter data by:

* Fuel Type
* Payment Mode
* Location
* Shift
* Date

---

# 🔍 Key Insights

### Revenue Performance

The petrol pump network generated **₹10.83M in total revenue** during the analysis period.

### Fuel Demand

Petrol contributes the **largest share of fuel sales**, followed by diesel and premium petrol.

### Payment Behavior

Digital payments such as **UPI and card transactions are widely used**, indicating increasing adoption of cashless payments.

### Employee Performance

Some employees consistently generate **higher sales revenue**, indicating strong operational performance.

### Pump Performance

Revenue varies across petrol pump locations, highlighting **top-performing pumps and lower-performing outlets**.

### Shift Trends

The **evening shift generates the highest sales**, suggesting peak fuel demand during this time.

### Sales Trend

Revenue remains **relatively stable across the year**, with occasional spikes indicating higher fuel demand on certain days.

---

# 💡 Business Recommendations

Based on the analysis:

* Increase staffing during **evening shifts** to handle higher demand
* Encourage **digital payment adoption** for faster transactions
* Monitor lower-performing pumps for operational improvements
* Implement promotions during **low-demand periods**
* Reward high-performing employees to maintain productivity

---

# 🛠 Tools & Technologies

| Tool        | Purpose                                   |
| ----------- | ----------------------------------------- |
| Power BI    | Data visualization and dashboard creation |
| Power Query | Data cleaning and transformation          |
| DAX         | KPI calculations and metrics              |
| Excel       | Data storage and preparation              |

---

# 📷 Dashboard Preview

Example sections in the dashboard:

* Revenue Trend Analysis
* Pump Performance
* Employee Sales Comparison
* Fuel Distribution
* Payment Mode Analysis

*(Add screenshots of your dashboard here)*

---

# 🚀 How to Use the Dashboard

1. Download the `.pbix`
2. Open it in **Power BI Desktop**
3. Load the dataset
4. Use the slicers to explore sales insights interactively

---

# 📌 Project Outcomes

This project demonstrates the ability to:

* Perform **data cleaning and transformation**
* Create **data models and DAX calculations**
* Build **interactive dashboards**
* Extract **business insights from transactional data**

---

# 👨‍💻 Author

**Naveen Bolli**

Data Analyst | Power BI | Data Visualization | Business Analytics

---

⭐ If you like this project, feel free to **star the repository**.

---
