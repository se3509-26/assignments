# SE3509 – Week 03 PreLab: Statistical Thinking, Distributions & Data Visualization with Seaborn

## 📌 Course & Assignment Information

* **Course:** SE3509
* **Assignment:** PreLab 03 – Conceptual Analysis: Statistical Distributions & Exploratory Visualization
* **DataCamp Career Track:** [Associate Data Scientist in Python](https://app.datacamp.com/learn/career-tracks/associate-data-scientist-in-python)
* **Track Modules Covered:**
  * **Module 5:** *Introduction to Statistics in Python*
  * **Module 6:** *Introduction to Data Visualization with Seaborn*
* **Central Announcement Repo:** [https://github.com/se3509-26/assignments](https://github.com/se3509-26/assignments)
* **Submission Platform:** **DYS (Ders Yönetim Sistemi)**  
  *(Ödev teslimleri doğrudan Üniversite DYS sistemi üzerinden yüklenecektir.)*
* **Submission Deliverable:** Microsoft Word document (`.docx`) containing your accessible OneDrive sharing link at the top.
* **File Naming Convention:** `studentNo_surname_name_SE3509_PreLab03.docx`
* **Submission Deadline:** **Tuesday, October 13, 2026 at 23:59**

> [!IMPORTANT]
> **Submission Policy:**  
> This assignment is announced on GitHub for review and instructions. You must submit your completed Microsoft Word report (`.docx`) directly to the **DYS (Ders Yönetim Sistemi)** submission portal before the deadline. Ensure your OneDrive view/download link is pasted at the top of your document.

---

## 🎯 Workflow for Students

1. **Review:** Read the conceptual evaluation question below in the central `assignments` repository.
2. **Prepare:** Answer the questions in your own words using Microsoft Word based on the report template provided at the bottom of this document. Include relevant Python/pandas/seaborn code snippets where helpful.
3. **Submit:** Upload your `.docx` file named `studentNo_surname_name_SE3509_PreLab03.docx` to the **DYS** portal before **October 13, 2026, 23:59**.

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

## 📄 DYS Submission Template

Copy and paste the template below into your Microsoft Word document (`.docx`), write your answers, and upload it to **DYS (Ders Yönetim Sistemi)**:

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
• Submission Date: [13/10/2026]
• OneDrive View/Download Link: [Paste Your Accessible OneDrive Sharing Link Here]

--------------------------------------------------------------------------------
IMPORTANT NOTICE:
Submission Platform: DYS (Ders Yönetim Sistemi)
Submission Deadline: October 13, 2026, 23:59.
Format: Microsoft Word (.docx) with active OneDrive link.
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
