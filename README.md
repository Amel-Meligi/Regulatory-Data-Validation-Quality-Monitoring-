# 📊 Regulatory Data Validation & Quality Monitoring  
**Python | Pandas | Data Quality | Regulatory Analytics**

---

## 📌 Project Overview

In regulated industries such as pharmaceuticals, **data accuracy is not optional**.  
Inconsistent or incomplete regulatory data can lead to reporting errors, audit findings, and delayed business decisions.

This project demonstrates how **Python can be used to validate, clean, and prepare regulatory submission data** before it is consumed by analytics and BI tools such as Power BI.

The focus is on **data quality, business rules, and audit readiness** — a critical responsibility of data analysts working in regulated environments.

---

## 🎯 Business Problem

Regulatory teams often rely on manually maintained Excel files to track:

- Submission status  
- Approval timelines  
- Workload distribution  
- Compliance readiness  

Over time, these datasets accumulate issues such as:
- Missing approval dates  
- Invalid date sequences  
- Status inconsistencies  
- Long approval delays  

Without systematic validation, these issues silently propagate into reports and dashboards.

---

## 🧠 Solution Approach

This project implements a **Python-based data validation pipeline** that:

1. Loads raw regulatory submission data  
2. Applies real-world **regulatory business rules**  
3. Flags data quality issues instead of deleting records  
4. Produces:
   - A clean, analytics-ready dataset  
   - A management-ready data quality report  

This mirrors how data analysts support **compliance, reporting, and decision-making** in real organizations.

---

## 🗂 Dataset Description

The dataset represents **simulated regulatory submission data**, designed to reflect real-world pharmaceutical regulatory processes.

Each row represents a single regulatory submission.

**Key fields include:**
- Submission and approval dates  
- Submission status (Approved / Under Review / Rejected)  
- Regulatory authority  
- Submission type and variation category  
- Assigned employee  

> ⚠️ The dataset is intentionally messy and contains realistic errors to demonstrate data validation logic.  
> No confidential or real company data is used.

---

## ✅ Data Quality Rules Implemented

The following validation checks are applied:

1. Approved submissions must have an approval date  
2. Approval date cannot be earlier than submission date  
3. Rejected submissions should not contain approval dates  
4. Approval duration greater than 180 days is flagged as a potential delay risk  

Each rule is implemented as a boolean flag to ensure transparency and auditability.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- CSV / Excel file handling  

---

## 📂 Project Structure

regulatory-data-validation/
│
├── data/
│ └── regulatory_submissions_raw.csv
│
├── scripts/
│ └── data_validation.py
│
├── outputs/
│ ├── regulatory_submissions_clean.csv
│ └── data_quality_report.xlsx
│
└── README.md


---

## 📈 Outputs

### 1️⃣ Clean Dataset  
**`regulatory_submissions_clean.csv`**

- Includes original data  
- Adds validation flags  
- Adds approval duration metric  
- Ready for Power BI or further analysis  

---

### 2️⃣ Data Quality Report  
**`data_quality_report.xlsx`**

Summarizes:
- Number of records affected by each data quality issue  
- Percentage of total records  

Useful for management reporting and audit preparation.

---

## 🖼 Screenshots

Create a `screenshots/` folder and add the following images.

### 🔹 Data Quality Report
![Data Quality Report](screenshots/data_quality_report.png)

### 🔹 Clean Dataset Preview
![Clean Dataset Preview](screenshots/clean_dataset_preview.png)

---

## 🔗 How This Fits Into a BI Workflow

This project represents the **upstream data preparation step** in a typical analytics pipeline:

**Python → SQL / Power BI → Dashboard → Business Decision**

The clean dataset produced here can be directly consumed by Power BI for:
- Regulatory performance monitoring  
- Delay and risk analysis  
- Workload distribution reporting  

---

## 💼 Why This Project Matters

This project demonstrates:
- Real-world data cleaning (not toy datasets)  
- Business rule implementation  
- Regulatory and compliance awareness  
- Analytics thinking beyond visualization  

It reflects the responsibilities of a **Data Analyst or Power BI Developer in regulated industries**.

---

## 👤 Author

**Amel Meligi**  
Data Analyst | Power BI Developer  
Background in Pharmaceutical Regulatory Affairs  

🔗 LinkedIn: https://www.linkedin.com/in/amel-meligi  
🔗 GitHub: https://github.com/Amel-Meligi  
