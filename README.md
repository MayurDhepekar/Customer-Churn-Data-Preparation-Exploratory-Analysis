
---

## 🚀 Objectives

### ✅ 1. Import & Quality Assurance
- Imported customer and account data from two Excel sheets using `pandas`.
- Merged them with a **left join on `CustomerId`**.
- Removed **duplicate rows** (4 in total) and redundant columns.

### ✅ 2. Data Cleaning
- **Data Types Fixes:** Converted currency fields like `Balance` and `EstimatedSalary` from string (e.g., "€123.45") to float.
- **Missing Value Handling:**
  - Replaced categorical NaNs with `"MISSING"`.
  - Replaced numeric NaNs and nonsensical values (e.g., `-999999`) with **median**.
- **Label Standardization:** Unified inconsistent geography labels like `"FRA"`, `"French"` → `"France"`.

### ✅ 3. Exploratory Data Analysis (EDA)
- Created a **bar plot** of churn distribution (`Exited` column).
- Analyzed churn by **Geography** and **Gender**.
- Built **box plots** and **histograms** for numeric columns grouped by churn status.

### ✅ 4. Data Preparation for Modeling
- Dropped ID-based and non-informative columns (e.g., `Surname`, `CustomerId`).
- Generated **dummy variables** for categorical fields.
- Engineered a new feature:  
  `balance_v_income = Balance / EstimatedSalary`
- Visualized this ratio against churn to discover feature relevance.

---

## 🔧 Tech Stack
- **Python 3.9**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Jupyter Notebook**

---

## 📊 Key Insights
- Customers from certain geographies and age groups had higher churn rates.
- Outliers and missing data had significant influence on churn trends.
- Feature `balance_v_income` showed meaningful separation between churners and non-churners.

---

## 🧠 Skills Demonstrated
- Real-world data cleaning & transformation
- Handling missing and incorrect data
- Exploratory visualizations for pattern discovery
- Feature engineering for model-readiness

---

## 📂 Dataset Source
The dataset is fictional and used for practice purposes, simulating a real-world bank churn problem.

---

## 📌 Next Steps (Future Scope)
- Apply Logistic Regression or Decision Trees for churn prediction.
- Use SMOTE or similar methods for class imbalance.
- Build a dashboard using Power BI or Streamlit for stakeholder reporting.

---

## 📫 Contact
**Mayur Dhepekar**  
📧 mayurdehpekar00@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/mayurdhepekar/)  
🌐 [Portfolio](https://mavenanalytics.io/profile/78b16390-c051-70d2-5fed-5d6c90192ca3)

---

> ⭐ If you found this project helpful, feel free to fork, star, or connect!
