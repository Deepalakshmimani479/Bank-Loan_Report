
# 📊 Driver Behavior & Fleet Efficiency Analysis (Excel Project – No Visualization)

## 📌 Project Summary
This Excel-based project analyzes trip-level data to evaluate driver behavior and vehicle usage patterns. The focus is on **data cleaning**, **formula-based insights**, and **Pivot Table analysis** — without charts or dashboards.

---

## 🧩 Dataset Overview

The dataset contains 10,000 rows and includes:

| Column       | Description                              |
|--------------|------------------------------------------|
| `Driver`     | Driver name (may be blank or “Unknown”)  |
| `Distance`   | Trip distance (some with "km" text)      |
| `Brake`      | Harsh braking event count                |
| `Accel`      | Acceleration event count                 |
| `Speed`      | Speeding indicator or count              |
| `Time_Min`   | Duration of trip in minutes              |
| `Date`       | Trip date (varied formats)               |
| `Note`       | Manual entry, optional                   |

---

## 🎯 Business Questions Answered

1. **Which drivers show the most risky behavior?**  
   → Based on harsh braking, acceleration, and speeding

2. **How does driver behavior vary per day/week?**  
   → Grouped using Excel date functions and Pivot Table

3. **Which driver has the highest average driving time or distance?**

4. **How many trips did each driver make?**

5. **What is the count of missing fields per driver across distance, brake, and time?**

---

## 🛠 Excel Techniques Used

- **Data Cleaning**
  - Removed "km" units from distance using `VALUE()` + `LEFT()`
  - Converted mixed date formats using `DATEVALUE()` and `TEXT()`
  - Replaced blank names with `"Unknown"` using `IF()`

- **Formulas**
  - `IF()`, `IFERROR()`, `ISNUMBER()`, `COUNTIFS()`, `XLOOKUP()`
  - Helper columns to detect missing fields

- **Pivot Table Analysis**
  - Grouped dates by week
  - Calculated averages per driver
  - Counted missing data entries per person

---

## ✅ Key Findings

- Some drivers like **"Unknown"** had many missing or incomplete records
- A few drivers showed frequent harsh events (brake/accel)
- Weekday vs weekend behavior patterns were observed
- Several trips had idle times but little distance → inefficiency risk

---

## 📁 Files

| File Name                         | Description                            |
|----------------------------------|----------------------------------------|
| `Cleaned_Driver_Data.xlsx`       | Final cleaned dataset + formulas       |
| `Driver_Analysis_Pivot.xlsx`     | Pivot Table analysis (no visuals)      |
| `README.md`                      | This documentation                     |

---

## 👤 Author

**Deepalakshmi Mani**  
_Aspiring Data Analyst | Excel Projects | Clean Data_
