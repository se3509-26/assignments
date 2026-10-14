# SE3509 – Week 03 PreLab: Statistical Thinking, Distributions & Data Visualization with Seaborn

## 📌 Course & Assignment Information

* **Course:** SE3509
* **Assignment:** PreLab 03 – Conceptual Analysis: Statistical Distributions & Exploratory Visualization
* **DataCamp Career Track:** [Associate Data Scientist in Python](https://app.datacamp.com/learn/career-tracks/associate-data-scientist-in-python)
* **Track Modules Covered:**
  * **Module 5:** *Introduction to Statistics in Python*
  * **Module 6:** *Introduction to Data Visualization with Seaborn*
* **Central Assignment Repo:** [https://github.com/se3509-26/assignments](https://github.com/se3509-26/assignments)
* **Student Target Repo:** Your private student repository (`Lab_se-XXXXXXXXX` / `Labse-XXXXXXXXX`)
* **Submission Deadline:** **Tuesday, October 13, 2026 at 23:59**
* **Submission Deliverable:** Microsoft Word document (`.docx`) placed under `week03/` or `prelab03/` in your private lab repository + OneDrive sharing link.
* **File Naming Convention:** `studentNo_surname_name_SE3509_PreLab03.docx`

> [!CAUTION]
> **Mandatory Completion Policy:**  
> Submitting this PreLab report before the deadline (**October 13, 2026, 23:59**) is **mandatory**. Students who fail to complete and commit their report to their private repository on time will receive **0 points (no lab grade)** for this lab session.

---

## 🎯 Workflow for Students

1. **Review:** Read the conceptual evaluation question below in the central `assignments` repository.
2. **Prepare:** Answer the questions in your own words using Microsoft Word based on the report template provided at the bottom of this document. Include relevant Python/pandas/seaborn code snippets where helpful.
3. **Commit & Push:** Save your `.docx` file as `studentNo_surname_name_SE3509_PreLab03.docx` inside the `week03/` folder in your private student repository (`Lab_se-XXXXXXXXX`), then commit and push to GitHub:
   ```bash
   cd Lab_se-XXXXXXXXX
   mkdir -p week03
   # Place your studentNo_surname_name_SE3509_PreLab03.docx file into week03/
   git add week03/
   git commit -m "week03: submit prelab 03 report"
   git push origin main
   ```

---

## ❓ PreLab Conceptual Questions

---

### Question 1 (DataCamp Track Course 5: *Introduction to Statistics in Python*)
**Topic:** Statistical Measures of Spread, Central Limit Theorem (CLT), and Correlation vs. Causation

1. **Robustness of Central Tendency & Dispersion:**
   * Compare **Mean** vs. **Median** and **Standard Deviation** vs. **Interquartile Range (IQR)** when dealing with heavily right-skewed real-world data (such as web server latency or user income).
   * Why do extreme outliers distort the Mean and Standard Deviation, and why are Median and IQR considered robust non-parametric metrics?
2. **The Central Limit Theorem (CLT) & Inferential Decisions:**
   * Formulate the **Central Limit Theorem (CLT)** in your own words.
   * Why does the distribution of sample means approach a **Normal (Gaussian) Distribution** even if the underlying population distribution is non-normal (e.g., highly skewed, exponential, or uniform)?
   * Explain why the CLT is considered the cornerstone of modern data science A/B testing and confidence interval estimations.
3. **Correlation Dynamics & Simpson's Paradox:**
   * Contrast **Pearson Correlation Coefficient ($r$)** with **Spearman Rank Correlation ($\rho$)**. In what data engineering scenarios (e.g., non-linear monotonic relationships or ordinal scales) does Spearman outperform Pearson?
   * Define **Simpson's Paradox**. Construct a realistic data scenario where an aggregate positive correlation between two variables completely reverses (or disappears) when the dataset is stratified into subgroups by a confounding variable.

---

### Question 2 (DataCamp Track Course 6: *Introduction to Data Visualization with Seaborn*)
**Topic:** Exploratory Data Analysis (EDA), Statistical Distributions & Visual Multi-Dimensional Faceting

1. **Distribution Visualization & Pitfalls:**
   * Compare **Box Plots (`sns.boxplot()`)**, **Histograms with Kernel Density Estimation (`sns.histplot(kde=True)`)**, and **Violin Plots (`sns.violinplot()`)**.
   * Explain why a standard Box Plot can be deceptively blind to bimodal or multimodal distributions (e.g., two distinct population clusters), and how a Violin Plot or KDE plot reveals the underlying density structure.
2. **Multi-Dimensional Visual Encoding with Seaborn:**
   * Contrast Seaborn's high-level figure-level functions (e.g., `sns.relplot()`, `sns.catplot()`) with lower-level axes-level functions (e.g., `sns.scatterplot()`, `sns.barplot()`).
   * How do semantic aesthetic mappings—such as **`hue`**, **`style`**, **`size`**, along with subplot faceting (**`col`**, **`row`**)—allow data scientists to visualize up to 5 dimensions in a single plot without confusing the audience?
3. **Visual Integrity in Data Science:**
   * Explain how truncating the y-axis (not starting at zero for bar charts) or using an inappropriate linear scale instead of a logarithmic scale for exponential data can mislead decision-makers.

---

## 📄 Word (.docx) Submission Template

Copy and paste the template below into your Microsoft Word document:

```text
================================================================================
                        MUĞLA SITKI KOÇMAN UNIVERSITY
                            FACULTY OF ENGINEERING
                       DEPARTMENT OF SOFTWARE ENGINEERING
                     SE3509 - PRELAB 03 EVALUATION REPORT
================================================================================

STUDENT INFORMATION:
• Full Name: [Your Name and Surname]
• Student ID: [Your Student ID]
• GitHub Username: se-[Your Student ID]
• Private Lab Repo: https://github.com/se3509-26/Lab_se-[Your Student ID]
• Submission Date: [13/10/2026]
• OneDrive View/Download Link: [Insert Link - View & Download Only]

--------------------------------------------------------------------------------
IMPORTANT NOTICE:
Submission Deadline: October 13, 2026, 23:59.
Failure to submit this PreLab report by the deadline results in 0 points 
(no lab grade) for this lab session.
--------------------------------------------------------------------------------

SECTION 1: CONCEPTUAL EVALUATION QUESTIONS

[QUESTION 1: Statistical Measures, Central Limit Theorem & Simpson's Paradox]
Your Answer:
(Provide a detailed explanation comparing Mean/Median and StdDev/IQR on skewed data, 
formulate the Central Limit Theorem and its importance in A/B testing, and explain 
Pearson vs. Spearman correlation along with Simpson's Paradox.)


[QUESTION 2: Seaborn Statistical Visualizations & Multi-Dimensional Faceting]
Your Answer:
(Compare Box Plots vs Violin Plots vs KDE for multimodal data, explain Seaborn 
aesthetic mappings hue/style/size/col/row in high-dimensional EDA, and discuss 
visual integrity and scaling choices.)


--------------------------------------------------------------------------------

SECTION 2: KEY TAKEAWAYS & DATA SCIENCE INSIGHTS
• Summarize the two most critical statistical and visualization insights you gained 
  and how they apply to end-to-end data science pipelines (2–3 sentences):
  [Your Summary...]

================================================================================
```
