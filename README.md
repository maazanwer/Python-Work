# Data Cleaning & Profiling Project

## Project Overview
This project demonstrates the complete cleaning process of a dataset containing **216 rows** and **48 columns**.  
The primary goal was to **prepare the data for analysis** by removing unnecessary columns, standardizing names, and applying targeted cleaning rules based on domain knowledge.

---

## Steps Performed

### 1️⃣ Column Standardization
- Removed irrelevant columns.
- Standardized column names using `.strip()` and `.lower()` to ensure consistency.

### 2️⃣ General Data Cleaning
- Removed leading/trailing spaces in string values.
- Handled missing values and replaced inconsistent entries.

### 3️⃣ Targeted Column-by-Column Cleaning
- Applied **domain knowledge** to correct data based on dependencies:
  - If `employment_status` = `"no"`, then `organization`, `work_hours`, `income`, and `taxpayer_status` were set to `"unemployed"`.
  - If `children` = `"no"`, then `children_age` was set to `"no child"`.
  - Similar logical corrections applied to related fields.

### 4️⃣ Data Profiling
- Used **ydata-profiling** to generate **before** and **after** profiling reports.
- Key improvements included:
  - Removal of inconsistent entries.
  - Reduction of missing values to 0%.
  - Clearer categorical distributions.

---

## Visual Summary
The project includes **5 before-and-after visual comparisons**:
1. **Overview of the Dataset**
2. **Organizations**
3. **Siblings**
4. **Ethnicity**
5. **Summary Table**


---

## 🚀 Tools Used
- **Python**
- **Pandas**
- **ydata-profiling**
- **Matplotlib / Seaborn** (for additional visuals)

---

## 📢 Note
Data is confidential, so only the **cleaning process and structure** are shared.
