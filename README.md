# 🛍 Black Friday Sales Data Analysis

## 📂 Dataset Details
- **Dataset Name:** Black Friday Sales Data  
- **Dataset Size:** 23 MB CSV file (~537,000 rows, 12 columns)  
- **Columns:**  
  - User ID  
  - Product ID  
  - Gender  
  - Age  
  - Occupation  
  - City Category  
  - Stay in Current City Years  
  - Marital Status  
  - Product Categories (1, 2, 3)  
  - Purchase Amount  
- **Source:** Public Dataset (Available on GitHub)  


---

## 📊 Project Steps Overview

### 1️⃣ Walkthrough of the Dataset
**Goal:** Load the dataset, inspect its structure, and understand the contents.  
**Actions:**  
- Load the dataset into a Pandas DataFrame.  
- Check for missing values and discrepancies.  
- Use `df.info()` to inspect column types and non-null counts.  


---

### 2️⃣ Analyzing Columns
**Goal:** Understand each column’s distribution and relevance.  
**Actions:**  
- Focus on key columns: `Gender`, `Age`, `Marital_Status`, `Product_Category`, `Purchase`.  
- Remove sparse columns (`Product_Category_2` & `Product_Category_3`).  
- Use `.unique()` and `.nunique()` to get unique values of columns.  



---

### 3️⃣ Analyzing Gender
**Goal:** Examine gender distribution and purchase patterns.  
**Actions:**  
- Found **data imbalance**: more male customers than female.  
- Used `groupby()` to show male customers made more total purchases.  


---

### 4️⃣ Analyzing Age & Marital Status
**Goal:** Analyze purchasing behavior across age groups and marital status.  
**Actions:**  
- Group data by `Age` and `Marital_Status`.  
- Identified which demographic groups spent more during Black Friday sales.  


---

### 5️⃣ Multi Column Analysis
**Goal:** Combine factors for deeper insights.  
**Actions:**  
- Combined `Age`, `Marital_Status`, `Gender` to detect patterns.  
- Used **Pie Charts** & **Bar Plots** for visualization.  



---

### 6️⃣ Occupation & Products Analysis
**Goal:** Understand product preferences by occupation.  
**Actions:**  
- Analyzed `Occupation`, `Product_ID`, `Product_Category_1`.  
- Mapped relationships between occupation type and purchased product category.  



---

### 7️⃣ Combining Gender & Marital Status
**Goal:** See if gender & marital status jointly affect purchases.  
**Actions:**  
- Used Seaborn `countplot` to visualize the relationships.  
- Found combinations that purchased more frequently.  



---

## ✅ Conclusion
This project explored **Black Friday shopping behavior** by analyzing demographic factors such as **gender, age, marital status, occupation, and product categories**.  
We performed:
- **Data Cleaning**
- **Column-wise Analysis**
- **Multi-column Relationship Analysis**
- **Visualization of Patterns** with Matplotlib & Seaborn  

**Key Takeaways:**
- Males outnumber females in the dataset and contribute more to purchases.  
- Certain age groups and occupations spend significantly more.  
- Combining demographic factors reveals **hidden trends** in purchasing behavior.  

---

📌 *This README provides an overview of the Black Friday Data Analysis project. Each step is available in the linked Jupyter Notebooks for further exploration.*
