# New-York-City-s-Crime-Analysis-using-Python-and-Power-BI
files are in drive link

## 📊 Crime Against Women Analysis (2017–2019)
This project focuses on analyzing crime incidents involving female victims in New York City from 2017 to 2019. The goal is to uncover patterns in crime types, locations, time of occurrence, and suspect demographics in order to better understand the risks women face in public and private spaces.

### 🔧 Tools Used
Power BI – For creating interactive dashboards and visualizing crime trends.
Python (Pandas, Matplotlib, Seaborn) – For data cleaning, preprocessing, and additional exploratory analysis.

### 📌 Key Insights
Harassment is the most frequently reported crime against women.
Streets and apartment houses are the most common crime locations.
Evening hours show the highest crime occurrence.
A large portion of suspects are unidentified, while known suspects are predominantly male.
Trends show a rise in crime cases in Q2 of 2019, indicating a need for stronger intervention.

### 🗂️ Files Included
Bibi_Nahida_Crime_Analysis.pbix – Power BI report file.
crime_analysis_nyc.py – Python script for data preprocessing and analysis.
nyc_crime_2015_2019.csv – Cleaned dataset used in Power BI.

images/ – Contains visuals used in the report.

### 🧠 Purpose
This project was developed to raise awareness about gender-based violence and assist in data-driven decision-making for public safety. It combines data analytics and storytelling to highlight the real-world impact of crimes against women.

### 🔍 Key Fields Used
CMPLNT_FR_DT – Date of the crime report.
OFNS_DESC – Description of the offense.
VIC_SEX – Gender of the victim (filtered for FEMALE).
SUSP_SEX – Gender of the suspect.
PREM_TYP_DESC – Location type (e.g., street, residence).
CRM_ATPT_CPTD_CD – Whether the crime was attempted or completed.
LAW_CAT_CD – Classification (Felony, Misdemeanor, Violation).
KY_CD – Offense code (used for grouping crimes).

### 🧹 Data Cleaning
Filtered data to include only crimes against female victims.
Removed null or irrelevant records.
Grouped and reclassified certain offenses (e.g., minor/major assault).
Created new features (e.g., time of day, crime quarter).
Cleaned and simplified offense descriptions for analysis and visualization.

### 📊 Dataset Size
Total Records Used: ~1,400,000 (after filtering for 2017–2019)
