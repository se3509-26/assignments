# SE3509 – Week 01 PreLab: Python & Pandas Conceptual Analysis

## 📌 Course & Assignment Information

* **Course:** SE3509
* **Assignment:** PreLab 01 – Conceptual Discussion Report
* **Central Assignment Repo:** [https://github.com/se3509-26/assignments](https://github.com/se3509-26/assignments)
* **Student Target Repo:** Your private student repository (`Lab_se-XXXXXXXXX` / `Labse-XXXXXXXXX`)
* **Submission Deadline:** **Tuesday, September 29, 2026 at 23:59**
* **Submission Deliverable:** Microsoft Word document (`.docx`) placed under `week01/` or `prelab01/` in your private lab repository + OneDrive sharing link.
* **File Naming Convention:** `studentNo_surname_name_SE3509_PreLab01.docx`

> [!CAUTION]
> **Mandatory Completion Policy:**  
> Submitting this PreLab report before the deadline (**September 29, 23:59**) is **mandatory**. Students who fail to complete and commit their report to their private repository on time will receive **0 points (no lab grade)** for this lab session.

---

## 🎯 Workflow for Students

1. **Review:** Read the questions below in the central `assignments` repository.
2. **Prepare:** Fill out your answers in Microsoft Word using the report template below.
3. **Commit & Push:** Save your `.docx` file as `studentNo_surname_name_SE3509_PreLab01.docx` inside the `week01/` folder in your private student repository (`Lab_se-XXXXXXXXX`), then commit and push to GitHub:
   ```bash
   cd Lab_se-XXXXXXXXX
   mkdir -p week01
   # Place your studentNo_surname_name_SE3509_PreLab01.docx file into week01/
   git add week01/
   git commit -m "week01: submit prelab 01 report"
   git push origin main
   ```

---

## ❓ PreLab Conceptual Questions

Answer the following three open-ended questions in detail in your Word report:

### Question 1 (Source: *Introduction to Python*)
**Topic:** Memory Architecture & Performance: Python Native Lists vs. NumPy Arrays

1. Compare Python built-in `list` and NumPy `ndarray` in terms of memory layout (pointers vs. contiguous memory blocks) and element type homogeneity.
2. Define the concept of **vectorization**. Explain the systemic and performance-related reasons why vectorized operations in NumPy are preferred over traditional Python `for` loops when handling large numeric datasets.
3. Explain the behavioral difference when applying the `* 2` operation on a Python list versus a NumPy array.

---

### Question 2 (Source: *Intermediate Python*)
**Topic:** Data Filtering Strategies: Iterative Loops vs. Boolean Indexing in Pandas

Suppose you have a tabular dataset containing 100,000 records and you need to filter rows matching multiple conditions (e.g., `age > 30` and `income > 50000`).

1. Contrast filtering this dataset using standard Python iterative loops (`for`/`if-else`) versus utilizing **Boolean Indexing (Boolean Masks)** or `.loc[]` in Pandas.
2. Evaluate both approaches in terms of execution speed, vectorization benefits, memory usage, and code readability. Why has Boolean Indexing become the industry standard in data analytics workflows?

---

### Question 3 (Source: *Data Manipulation with pandas*)
**Topic:** Aggregation & Reshaping: `groupby().agg()` vs. `pivot_table()` & Missing Value Handling

1. Compare Pandas `groupby().agg()` and `pivot_table()`. Explain their primary use cases, structural differences in output (hierarchical MultiIndex vs. two-dimensional matrix), and when to choose one over the other in real-world data pipelines.
2. Describe how Pandas aggregation functions (e.g., `mean()`, `sum()`, `count()`) handle missing data (`NaN` / `None`) by default during grouped operations, and discuss the analytical implications this may cause if left unmanaged.

---

## 📄 Word (.docx) Submission Template

Copy and paste the template below into your Microsoft Word document:

```text
================================================================================
                        MUĞLA SITKI KOÇMAN UNIVERSITY
                            FACULTY OF ENGINEERING
                       DEPARTMENT OF SOFTWARE ENGINEERING
                     SE3509 - PRELAB 01 EVALUATION REPORT
================================================================================

STUDENT INFORMATION:
• Full Name: [Your Name and Surname]
• Student ID: [Your Student ID]
• GitHub Username: se-[Your Student ID]
• Private Lab Repo: https://github.com/se3509-26/Lab_se-[Your Student ID]
• Submission Date: [DD/MM/YYYY]
• OneDrive View/Download Link: [Insert Link - View & Download Only]

--------------------------------------------------------------------------------
IMPORTANT NOTICE:
Submission Deadline: September 29, 2026, 23:59.
Failure to submit this PreLab report by the deadline results in 0 points 
(no lab grade) for this lab session.
--------------------------------------------------------------------------------

SECTION 1: CONCEPTUAL EVALUATION QUESTIONS

[QUESTION 1: Python Lists vs. NumPy Arrays]
Your Answer:
(Provide a detailed explanation in your own words regarding memory layout, 
type homogeneity, vectorization, and execution performance. Add short code 
snippets if necessary.)


[QUESTION 2: Boolean Indexing vs. Standard Python Loops]
Your Answer:
(Explain the differences between procedural iterative filtering and vectorized 
boolean indexing regarding performance, memory, and maintainability.)


[QUESTION 3: Pandas GroupBy, Aggregations & Pivot Tables]
Your Answer:
(Analyze groupby, agg, pivot_table use cases, multidimensional structures, 
and missing value handling in aggregation pipelines.)


--------------------------------------------------------------------------------

SECTION 2: KEY TAKEAWAYS & SUMMARY
• Summarize the two most important takeaways you gained from these topics and 
  how they apply to large-scale data engineering (2–3 sentences):
  [Your Summary...]

================================================================================
```
