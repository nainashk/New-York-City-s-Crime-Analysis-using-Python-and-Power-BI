# Newyork City Crime Analysis From 2017 2019

### 🗂️ Find the files Here:
- 📊 [Crime Analysis (Power BI)](https://drive.google.com/file/d/1zxhNB-jcN9XC_N2SdF935sRZTLHV2F5Y/view?usp=drive_link)  
- 🐍 [Crime Analysis (Python)](https://drive.google.com/file/d/1e_GKndvMxdqggDZU2TMknwEzu10qTBTr/view?usp=drive_link)  
- 🧾 [Dataset (Kaggle - NYC Crime Analysis)](https://www.kaggle.com/code/brunacmendes/new-york-crime-analysis)  

<p align="center">
  <img src="https://github.com/user-attachments/assets/001dee8c-8c25-48db-834d-426a4e6ed556" alt="Let's Dig Into It" width="600"/>
</p>

## 📊 NYC Crime Analysis (2017–2019) with Focus on Female Victims
This project explores reported crime data in New York City from 2017 to 2019 using Python and Power BI. The initial goal was to identify patterns across all types of crimes—by offense, time, location, and demographics. However, after early exploration, a notable trend emerged: a significantly higher number of female victims compared to male victims. This led to a deeper investigation into crimes specifically affecting women.

## 🧰 Tools & Technologies
**Power BI** – For dashboard design and interactive visualizations.
**Python** – For data cleaning, preprocessing, and exploratory analysis.
**NYC Open Data** – Source of raw NYPD complaint records.

## 🗃️ About the Data
The dataset used comes from the NYPD Complaint Data Historic and includes crime complaints filed from 2009 to 2019. The data contains over **6 million** records with details like crime type, time, location, and victim/suspect demographics. For, this analysis the data was filtered to only study last 3 years **2017 to 2019** with 1.4 million cases. 

### 🧹 Data Cleaning
Filtered data to include only crimes against female victims.
Removed null or irrelevant records.
Grouped and reclassified certain offenses (minor/major assault).
Created new features (time of day, crime quarter).
Cleaned and simplified offense descriptions for analysis and visualization.

### 📊 Dataset Size
Total Records Used: ~1,400,000 (after filtering for 2017–2019)

### 🔎 Phase 1: General Crime Insights
In the first phase, the project examined crime trends across NYC:
Top Offenses: Theft and harassment were among the most common.
Location Patterns: Most crimes occurred on streets, followed by residential areas.
Time Trends: Crime peaks in the evening hours.
Suspect Demographics: Males made up the majority of identified suspects **while keeping in mind that most of the suspects data was missing**.

These insights helped create a foundation for exploring more focused topics within the data.

### 🚨 Phase 2: Focused Analysis – Crimes Against Women
After observing that **female victims were disproportionately affected**, the project shifted to spotlight crimes involving female victims only. The data was filtered to only cases with females victims with 400,000 cases.

#### 🔍 Key Findings
**Most Common Crime:** Harassment, followed by minor assault and theft.
**Top Locations:** Streets and apartment buildings pose the highest risk.
**Time of Day:** Evenings (33.2%) are the most dangerous for women, but crimes happen throughout the day.
**Suspect Info:** Nearly half of all cases had unknown suspects. Where known, most were male.
**Trend Over Time:** Cases increased into mid-2019, with the second quarter being the most active.
These findings raise concerns about women's safety in public and residential areas and stress the need for better prevention, identification, and reporting practices.



