# SE3509 – Week 02 PreLab: Relational Data Integration, Tidy Data Transformation & Feature Engineering

## 📌 Course & Assignment Information

* **Course:** SE3509
* **Assignment:** PreLab 02 – Conceptual Discussion & Data Engineering Pipeline Analysis
* **Central Assignment Repo:** [https://github.com/se3509-26/assignments](https://github.com/se3509-26/assignments)
* **Student Target Repo:** Your private student repository (`Lab_se-XXXXXXXXX` / `Labse-XXXXXXXXX`)
* **Submission Deadline:** **Tuesday, October 6, 2026 at 23:59**
* **Submission Deliverable:** Microsoft Word document (`.docx`) placed under `week02/` or `prelab02/` in your private lab repository + OneDrive sharing link.
* **File Naming Convention:** `studentNo_surname_name_SE3509_PreLab02.docx`

> [!CAUTION]
> **Mandatory Completion Policy:**  
> Submitting this PreLab report before the deadline (**October 6, 2026, 23:59**) is **mandatory**. Students who fail to complete and commit their report to their private repository on time will receive **0 points (no lab grade)** for this lab session.

---

## 🎯 Workflow for Students

1. **Review:** Read the questions below in the central `assignments` repository.
2. **Prepare:** Fill out your answers in Microsoft Word using the report template provided at the bottom of this document.
3. **Commit & Push:** Save your `.docx` file as `studentNo_surname_name_SE3509_PreLab02.docx` inside the `week02/` folder in your private student repository (`Lab_se-XXXXXXXXX`), then commit and push to GitHub:
   ```bash
   cd Lab_se-XXXXXXXXX
   mkdir -p week02
   # Place your studentNo_surname_name_SE3509_PreLab02.docx file into week02/
   git add week02/
   git commit -m "week02: submit prelab 02 report"
   git push origin main
   ```

---

## ❓ PreLab Conceptual Questions

Answer the following three open-ended questions in detail in your Word report:

### Question 1: Relational Data Joins & Schema Merging: `pd.merge()` vs. `pd.concat()`
**Topic:** Relational Algebra, Join Types, Key Collisions, and Cartesian Explosions

1. Compare `pd.merge()` and `pd.concat()`. Under what data engineering conditions should you prefer column/row-wise concatenation over relational key matching?
2. Explain the fundamental differences between the four primary join types in Pandas:
   * **Inner Join (`how='inner'`)**
   * **Left Outer Join (`how='left'`)**
   * **Right Outer Join (`how='right'`)**
   * **Full Outer Join (`how='outer'`)**  
   What happens when there are non-unique (duplicate) keys in both dataframes (e.g., $M$ matching keys on the left and $N$ on the right)? How does this lead to unexpected row count explosions (Cartesian products) and memory spikes?
3. How does merging on DataFrame indices (`left_index=True`, `right_index=True`) compare to merging on explicit columns in terms of computational efficiency and syntax?

---

### Question 2: Data Reshaping & Tidy Data Principles: `pd.melt()` vs. `pd.pivot()`
**Topic:** Normalization, Wide vs. Long Formats, and Analysis-Ready Data

1. Define Hadley Wickham’s **Tidy Data** principles:
   * Each variable forms a column.
   * Each observation forms a row.
   * Each type of observational unit forms a table.  
   Why is Tidy (Long-format) data significantly easier to manipulate with vectorized operations and statistical visualization libraries (such as Seaborn / Plotly) compared to untidy (Wide-format) data?
2. Contrast `pd.melt()` (unpivoting / wide-to-long) and `DataFrame.pivot()` / `pd.pivot_table()` (pivoting / long-to-wide). Provide a realistic concrete scenario where converting from wide format to long format is necessary before running grouped aggregations.
3. What is the difference between `DataFrame.pivot()` and `DataFrame.pivot_table()` when duplicate index/column pairs exist?

---

### Question 3: Robust Missing Value Imputation, Outlier Handling & Feature Encoding
**Topic:** Data Cleaning Strategies, Robustness against Anomalies, and Feature Transformations

1. Contrast different strategies for handling missing values (`NaN`):
   * Row/column deletion (`dropna()`)
   * Statistical central tendency imputation (`mean` vs. `median` vs. `mode`)
   * Sequential filling (`ffill()` / `bfill()` for time-series)  
   Explain why imputing skewed distributions with the **median** is preferred over the **mean**.
2. Compare the **Interquartile Range (IQR)** method and the **Z-score** method for detecting and treating outliers. Which method is more robust when the dataset contains extreme skewness or heavy tails, and why?
3. When preparing categorical features for downstream analysis or machine learning:
   * When should you use **One-Hot Encoding** (`pd.get_dummies()`) vs. **Ordinal/Target Encoding**?
   * What issues arise when applying One-Hot Encoding on high-cardinality categorical variables (e.g., 5,000 distinct city names)?

---

## 📄 Word (.docx) Submission Template

Copy and paste the template below into your Microsoft Word document:

```text
================================================================================
                        MUĞLA SITKI KOÇMAN UNIVERSITY
                            FACULTY OF ENGINEERING
                       DEPARTMENT OF SOFTWARE ENGINEERING
                     SE3509 - PRELAB 02 EVALUATION REPORT
================================================================================

STUDENT INFORMATION:
• Full Name: [Your Name and Surname]
• Student ID: [Your Student ID]
• GitHub Username: se-[Your Student ID]
• Private Lab Repo: https://github.com/se3509-26/Lab_se-[Your Student ID]
• Submission Date: [06/10/2026]
• OneDrive View/Download Link: [Insert Link - View & Download Only]

--------------------------------------------------------------------------------
IMPORTANT NOTICE:
Submission Deadline: October 6, 2026, 23:59.
Failure to submit this PreLab report by the deadline results in 0 points 
(no lab grade) for this lab session.
--------------------------------------------------------------------------------

SECTION 1: CONCEPTUAL EVALUATION QUESTIONS

[QUESTION 1: Relational Data Joins & Schema Merging: pd.merge vs pd.concat]
Your Answer:
(Provide a detailed explanation comparing merge and concat, the 4 relational join 
types, duplicate key cartesian explosions, and index vs column merging efficiency.)


[QUESTION 2: Data Reshaping & Tidy Data Principles: pd.melt vs pd.pivot]
Your Answer:
(Explain Tidy Data theory, contrast pd.melt wide-to-long with pd.pivot long-to-wide, 
and explain duplicate handling in pivot vs pivot_table.)


[QUESTION 3: Robust Missing Value Imputation, Outlier Handling & Feature Encoding]
Your Answer:
(Analyze dropna vs statistical imputation mean/median, compare IQR vs Z-score outlier 
detection, and evaluate One-Hot vs Ordinal encoding for categorical columns.)


--------------------------------------------------------------------------------

SECTION 2: KEY TAKEAWAYS & SUMMARY
• Summarize the two most important data wrangling and integration techniques you learned 
  and how they apply to end-to-end data pipelines (2–3 sentences):
  [Your Summary...]

================================================================================
```
