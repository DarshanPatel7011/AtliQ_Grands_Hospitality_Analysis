# 🏨 AtliQ Grands Hospitality Analysis \| Power BI Dashboard

![Banner](./banner.png)

![Power BI](https://img.shields.io/badge/Tool-PowerBI-yellow)
![SQL](https://img.shields.io/badge/Language-SQL-blue)
![Excel](https://img.shields.io/badge/Tool-Excel-green)
![DAX](https://img.shields.io/badge/Skill-DAX-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

------------------------------------------------------------------------

## 📌 Project Overview

This project presents a **comprehensive Power BI dashboard** designed to
analyze the performance of *AtliQ Grands*, a luxury hotel chain across
India.

The dashboard enables stakeholders to monitor **Revenue, Occupancy,
Customer Ratings, Booking Trends, and Cancellations** to drive better
business decisions.

------------------------------------------------------------------------

## 🎯 Business Problem

AtliQ Grands has been facing:

-   📉 Declining market share\
-   💰 Revenue loss due to poor pricing strategies\
-   ❌ High cancellation rates (\~24%)\
-   📊 Lack of centralized analytics

👉 Goal: Build a **data-driven dashboard** to identify performance gaps
and improve decision-making.

------------------------------------------------------------------------

## 🧩 Data Model (Star Schema)

### 🔹 Fact Tables

-   `fact_bookings` → Booking-level transactional data\
-   `fact_aggregated_bookings` → Aggregated metrics (capacity,
    successful bookings)

### 🔹 Dimension Tables

-   `dim_date` → Date hierarchy (week, month, year)\
-   `dim_hotels` → Property details (city, hotel, category)\
-   `dim_rooms` → Room classification

### 🔹 Model Highlights

-   Optimized **one-to-many relationships**\
-   Supports fast filtering and drill-down analysis\
-   Built for scalability and performance

------------------------------------------------------------------------

## 🖼️ Dashboard Preview

### 🔹 Data Model

![Data Model](./0.Data%20Model.PNG)

### 🔹 Overall Analysis

![Overall Analysis](./1.Overall%20Analysis.PNG)

### 🔹 Monthly & Platform Analysis

![Monthly Analysis](./2.Monthly%20Analysis.PNG)

------------------------------------------------------------------------

## 📊 Key KPIs

  Metric                 Value
  ---------------------- ---------
  💰 Revenue             499.18M
  🏨 Occupancy           57.45%
  ⭐ Avg Rating          3.62
  ❌ Cancellation Rate   24.4%

------------------------------------------------------------------------

## 🔍 Key Insights

### 🔹 Revenue & Occupancy

-   Revenue reached **\~499M**, but occupancy is only **57%**
-   Indicates **underutilized capacity**

### 🔹 City Performance

-   🥇 Mumbai → Highest revenue\
-   ⭐ Delhi → Best ratings\
-   Balanced occupancy across cities

### 🔹 Property Insights

-   Top Performer: **AtliQ Exotica**\
-   Low Performer: **AtliQ Seasons**

### 🔹 Booking Platforms

-   Highest bookings: **Others & MakeMyTrip**\
-   Lowest: **Direct Offline**\
-   High cancellations across all platforms

### 🔹 Capacity vs Bookings

-   Large gap between **available rooms vs booked rooms**
-   Opportunity for pricing & marketing optimization

------------------------------------------------------------------------

## 🛠️ Tools & Technologies

-   **Power BI** -- Data visualization\
-   **Power Query** -- Data transformation\
-   **DAX** -- Calculations & KPIs\
-   **Excel / CSV** -- Data source

------------------------------------------------------------------------

## ⚙️ Key DAX Measures

``` dax
Revenue = SUM(fact_bookings[revenue_realized])

Occupancy % = 
DIVIDE(
    SUM(fact_bookings[successful_bookings]),
    SUM(fact_aggregated_bookings[capacity])
)

Cancellation Rate = 
DIVIDE(
    [Total Cancelled Bookings],
    [Total Bookings]
)

RevPAR = 
DIVIDE(
    [Revenue],
    SUM(fact_aggregated_bookings[capacity])
)
```

------------------------------------------------------------------------

## 🚀 Business Impact

✔ Identified **revenue leakage due to cancellations**\
✔ Highlighted **underutilized hotel capacity**\
✔ Enabled **property-level performance tracking**\
✔ Supported **data-driven pricing strategies**

------------------------------------------------------------------------

## 📈 Skills Demonstrated

-   Data Modeling (Star Schema)\
-   Advanced DAX\
-   Dashboard Design & UX\
-   Business Analysis

------------------------------------------------------------------------

## 📚 Learnings

-   Importance of structured data modeling\
-   Writing optimized DAX measures\
-   Translating business problems into analytics solutions

------------------------------------------------------------------------

## 🔗 How to Use

1.  Download the `.pbix` file\
2.  Open in Power BI Desktop\
3.  Use filters (City, Property, Platform)\
4.  Explore insights using interactive visuals

------------------------------------------------------------------------

## 🙋‍♂️ About Me

Transitioning from **11+ years MIS Executive experience** to a **Data
Analyst role**\
Skilled in: **Excel \| Power BI \| SQL \| Python**

------------------------------------------------------------------------

## 📬 Connect With Me

-   LinkedIn: (Add your link)\
-   Email: (Add your email)

------------------------------------------------------------------------

## ⭐ Support

If you found this project helpful, please ⭐ the repository!
