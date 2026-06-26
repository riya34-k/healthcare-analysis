📌 Problem Statement

Hospitals generate massive amounts of patient data daily. This project analyses a real-world healthcare dataset to answer critical questions: Which conditions are most common? Which cost patients the most? How long do patients stay? Are admissions growing over time? The goal is to transform raw patient records into actionable insights for hospital management and healthcare policy makers.

📂 Dataset

Source: Healthcare Dataset — Kaggle
Size: 55,500 rows × 15 columns
Period: 2019 – 2024
Features include: Patient Age, Gender, Blood Type, Medical Condition, Admission Type, Doctor, Hospital, Insurance Provider, Billing Amount, Discharge Date, Medication, Test Results

🛠️ Tools & Technologies

Category               Tools
Language               Python 3
Data Analysis          Pandas, NumPy
Data Visualisation     Matplotlib, Seaborn
Dashboard              Microsoft Power BI
Environment            VS Code

🔍 Project Workflow

1. Data Loading & Cleaning

Loaded 55,500 patient records using Pandas
Converted Date of Admission and Discharge Date to datetime format
Engineered new column: Length of Stay = Discharge Date − Admission Date
Removed 108 rows with negative billing amounts (data quality issue)
Standardised patient names to proper case (e.g., "bObBy jAcKsOn" → "Bobby Jackson")
Extracted Admission Year for yearly trend analysis
Final clean dataset: 55,392 rows

2. Exploratory Data Analysis (EDA)

Key questions answered through statistical analysis:

Question                                  Finding
Most common condition?                    Arthritis — 9,297 patients
Most expensive condition?                 Obesity — $25,860 avg billing
Longest hospital stay?                    Asthma — 15.7 days average
Most common admission type?               Elective — 18,618 patients
Test results breakdown?                   ~33% each — Abnormal, Normal, Inconclusive
Admissions trend?                         Spike in 2020, stable 2021–2023, drop in 2024 (incomplete year)

3. Python Visualisations

Generated 6 charts using Matplotlib and Seaborn:
Patients by Medical Condition (bar chart)
Average Billing Amount by Condition (bar chart)
Average Length of Stay by Condition (bar chart)
Yearly Patient Admissions Trend 2019–2024 (line chart)
Patient Test Results Distribution (bar chart)
Patient Age Distribution (histogram with KDE)


4. Power BI Dashboard

Built a 6-panel interactive dashboard in Power BI covering:
Patients by Medical Condition
Patient Gender Distribution
Patients by Admission Type
Average Billing by Medical Condition
Patient Test Results
Patients by Insurance Provider
