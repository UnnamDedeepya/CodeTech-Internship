
# 📦 Big Data Analysis – Amazon Unlocked Mobile Reviews

### 🎓 Internship Task: Big Data Analysis | Domain: Data Analysis  
🔧 Tools Used: PySpark, Google Colab, Pandas

---

## 📌 Objective

This task focuses on performing **Big Data Analysis** using `PySpark` on a real-world large-scale dataset of mobile product reviews. The goal is to:
- Clean and process messy data containing over 400,000 records
- Analyze brand trends, ratings, and pricing
- Handle data at scale using distributed computing practices

---

## 📊 Dataset Overview

**Name**: `Amazon_Unlocked_Mobile.csv`  
**Records**: ~413,000+  
**Columns**:
- `Product Name`: Name/model of the mobile phone
- `Brand Name`: Brand of the product
- `Price`: Sale price of the mobile
- `Rating`: User rating (1 to 5 stars)
- `Reviews`: Free-text customer review
- `Review Votes`: Number of helpfulness votes

---

## 🧹 Data Cleaning & Preparation

Several real-world issues were handled during preprocessing:

### 🔹 1. Malformed Rows
- Many rows contained **long unquoted reviews** with commas, causing misaligned data.
- Fixed using:
  ```python
  .option("multiLine", True).option("quote", '"').option("escape", '"')
  ```

### 🔹 2. Missing or Dirty Values
- Dropped rows with blank or missing `Brand Name` (~90K rows)
- Removed symbols and text from numeric columns using regex
- Casted `Price`, `Rating`, `Review Votes` to `DoubleType`
- Replaced missing numeric values with column mean
- Filled missing `Product Name` or `Review` fields with `"Unknown"`

### 🔹 3. Verified Clean Data
- Confirmed schema
- Validated numeric column conversions
- Exported cleaned dataset for reuse

---

## 🔍 Data Analysis & Insights

### ✅ 1. Top 10 Most Reviewed Brands
Identified brands like **Samsung, Apple, LG, Motorola** as the most reviewed.

### ✅ 2. Average Rating by Brand
Revealed:
- **Apple** and **OnePlus** consistently have high user satisfaction (avg rating ≥ 4.0)
- Budget brands like **Blu** also show strong user feedback

### ✅ 3. Average Price by Brand
- **Apple** leads with the highest average pricing
- **ZTE**, **BLU**, and **Nokia** trend in the budget segment

### ✅ 4. Rating Distribution
- Most ratings hover between **3.5 to 4.5**
- Low number of 1-star reviews indicates general product satisfaction

---

## 📁 Exported Results

Grouped analysis was exported as CSV files:
- `Average_Rating_By_Brand.csv`
- `Average_Price_By_Brand.csv`
- `Most_Reviewed_Brands.csv`

These offer downloadable insights from the cleaned dataset.

---

## ✅ Conclusion

This project demonstrates:
- Real-world Big Data cleaning with PySpark
- Handling messy textual data at scale
- Producing actionable insights from e-commerce product review data

> The approach and methodology reflect practical big data analytics in modern industry pipelines. This task simulates a scalable, professional-grade data workflow.

