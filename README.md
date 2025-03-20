# **🚖 Rides Data Analysis with Python**

This project explores **Uber ride data**, focusing on **Exploratory Data Analysis (EDA), Data Preprocessing, and Visualization** to uncover insights about **trip patterns, peak travel times, ride purposes, and distance distribution**.

---

## **Problem Statement**

Uber generates massive amounts of ride data daily, but understanding **ride trends, user behavior, and peak demand** remains a challenge.

This analysis aims to:

✅ Identify **peak travel times and most frequent ride purposes**.

✅ Understand **business vs. personal ride patterns**.

✅ Analyze **trip distances to optimize pricing strategies**.

✅ Provide **data-driven insights for ride-sharing optimization**.

---

## **📂 Project Structure**

```

Uber_rides
│-- Analysis.ipynb
│-- UberDataset.xlsx
│-- README.md

```

---

## **📊 Dataset Overview**

The dataset includes:

| Column Name | Description |
| --- | --- |
| `START_DATE` | Start time of the ride |
| `END_DATE` | End time of the ride |
| `CATEGORY` | Ride type (`Business` or `Personal`) |
| `START` | Pickup location |
| `STOP` | Drop-off location |
| `MILES` | Distance traveled (miles) |
| `PURPOSE` | Reason for the ride |

📌 **Key Statistics:**

- **Total rides analyzed:** 1156
- **Missing values handled:** `PURPOSE` column was filled with `"Unknown"`.
- **Duplicate records removed** for accurate analysis.

---

## **📈 Analysis & Insights**

### **1. Data Cleaning & Preprocessing**

- Converted **start and end dates** to the correct format.
- Filled missing values in the **PURPOSE** column.
- Extracted **date, time, and day-night classification** from `START_DATE`.
- Removed **duplicate records** to maintain data integrity.

### **2. Exploratory Data Analysis (EDA)**

- **Categorized rides into Business & Personal**.
- **Identified common ride purposes** (e.g., Meetings, Customer Visits).
- **Analyzed peak ride hours** (Morning, Afternoon, Evening).
- **Explored distance distribution** (Short vs Long rides).

### **3. Data Visualization**

- **Bar charts** for **CATEGORY** and **PURPOSE** distributions.
- **Time-based analysis** (Peak hours and monthly trends).
- **Heatmap of feature correlations** to detect relationships.
- **Distance distribution analysis** (Histograms & Boxplots).

---

## **📊 Key Insights**

📌 **Business rides dominate**: Most Uber rides were taken for business rather than personal use.

📌 **Most common ride purposes**: `Meetings` and `Customer Visits` were the top reasons for Uber usage.

📌 **Peak travel times**: Majority of rides occur in the **Afternoon (10 AM - 5 PM)**.

📌 **Shorter trips are more frequent**: Most rides cover a distance **between 4-5 miles**, and very few exceed **20 miles**.

📌 **Winter months (Nov, Dec, Jan) see a decline** in Uber ride counts.

---

## **Technologies Used**

- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical analysis
- **Matplotlib & Seaborn** – Data visualization
- **Scikit-learn** – OneHotEncoding for categorical variables
- **Jupyter Notebook** – Interactive coding environment
