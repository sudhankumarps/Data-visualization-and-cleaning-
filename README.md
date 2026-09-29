# Data Cleaning & Visualization Project (Healthcare)
**Internship Task — Data Science Domain**

## 📌 Objective
Take a raw, messy dataset, clean it (handle missing values, duplicates, and outliers), then visualize key insights using Python (Pandas, Matplotlib, Seaborn) and build a dashboard summarizing the findings.

## 📂 Files in this repo
| File | Description |
|---|---|
| `healthcare_raw_dataset.csv` | Raw, uncleaned dataset (350 patient records, with intentional missing values, duplicates, inconsistent text, and outliers) |
| `healthcare_cleaned_dataset.csv` | Final cleaned dataset after processing |
| `Healthcare_Data_Cleaning_Visualization.ipynb` | Full Jupyter notebook — cleaning steps, EDA, charts, and insights (already executed with outputs) |
| `Healthcare_Report.html` | Static HTML export of the notebook — viewable in any browser, no Jupyter needed |
| `healthcare_dashboard.html` | **Interactive dashboard** — KPI cards, filters (department/smoker), and 4 live charts |
| `Final_Report_Healthcare.docx` | Formal written report summarizing the task, methodology, and findings |

## 🖥️ How to view the dashboard
The interactive dashboard (`healthcare_dashboard.html`) is a self-contained HTML file — no server or installation needed:
1. Download `healthcare_dashboard.html` from this repo.
2. Double-click it (or right-click → Open with → your browser).
3. Use the Department/Smoker filters at the top to explore the data live.

A live hosted version is also available here: **[Interactive Dashboard](https://claude.ai/artifact/NwC4D8N4MdP2Q6SwnLeZjm)**

## 🧹 Cleaning steps performed
- Filled missing numeric values (Age, BMI, Blood Pressure, Cholesterol) with column medians
- Filled missing categorical values (Gender, Department, Smoker) with `'Unknown'`
- Standardized inconsistent text casing (e.g. `'male'` → `'Male'`)
- Removed duplicate rows
- Detected and capped outliers using the IQR method (e.g. age values above 150)

## 📊 Visualizations included
- Age distribution (histogram)
- Correlation heatmap (Age, BMI, Blood Pressure, Cholesterol, Length of Stay)
- Average length of stay by department (bar chart)
- BMI vs Cholesterol (scatter plot, by smoking status)
- Readmission rate by smoking status
- Combined 4-panel dashboard summary

## 💡 Key Insights
1. BMI and cholesterol show a positive relationship.
2. Length of stay varies noticeably by department.
3. Smokers show a higher readmission rate than non-smokers in this dataset.
4. Age distribution is fairly broad, covering young adults to elderly patients.
5. ~60–80% of the effort in a real data science task goes into cleaning, not modeling — this project reflects that.

## 🛠️ Tools used
Python · Pandas · NumPy · Matplotlib · Seaborn · Chart.js (for the interactive dashboard) · Jupyter Notebook

---
*Submitted as part of a Data Science internship task — Data Cleaning & Visualization Project.*
