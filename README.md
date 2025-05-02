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

## 🧰 Tools 
**Power BI** – For dashboard design and interactive visualizations.  
**Python** – For data cleaning, preprocessing, and exploratory analysis.  
**NYC Open Data** – Source of raw NYPD complaint records.  

## 🗃️ About the Data
The dataset used comes from the NYPD Complaint Data Historic and includes crime complaints filed from 2009 to 2019. The data contains over **6 million** records with details like crime type, time, location, and victim/suspect demographics. For, this analysis the data was filtered to only study last 3 years **2017 to 2019** with 1.4 million cases. 

### Data Dictionary
| **Column Name**     | **Data Type** | **Description**                                                                     |
| ------------------- | ------------- | ----------------------------------------------------------------------------------- |
| `CMPLNT_NUM`        | int64         | Unique identifier for each crime complaint.                                         |
| `CMPLNT_FR_DT`      | object (date) | Date the crime allegedly occurred.                                                  |
| `CMPLNT_FR_TM`      | object (time) | Time the crime allegedly occurred.                                                  |
| `CMPLNT_TO_DT`      | object (date) | End date of the crime occurrence (if it spans a range).                             |
| `CMPLNT_TO_TM`      | object (time) | End time of the crime occurrence (if it spans a range).                             |
| `ADDR_PCT_CD`       | float64       | Precinct code where the complaint was filed.                                        |
| `RPT_DT`            | object (date) | Date the complaint was officially reported.                                         |
| `KY_CD`             | int64         | Numeric offense classification code.                                                |
| `OFNS_DESC`         | object        | Description of the offense (e.g., ROBBERY, ASSAULT).                                |
| `PD_CD`             | float64       | NYPD internal classification code.                                                  |
| `PD_DESC`           | object        | NYPD internal offense description.                                                  |
| `CRM_ATPT_CPTD_CD`  | object        | Indicates whether the crime was completed (`COMPLETED`) or attempted (`ATTEMPTED`). |
| `LAW_CAT_CD`        | object        | Legal category: `FELONY`, `MISDEMEANOR`, or `VIOLATION`.                            |
| `BORO_NM`           | object        | Borough where the incident occurred (e.g., MANHATTAN, BROOKLYN).                    |
| `LOC_OF_OCCUR_DESC` | object        | Location description relative to the building (e.g., FRONT OF, INSIDE).             |
| `PREM_TYP_DESC`     | object        | Type of premises where the crime occurred (e.g., RESIDENCE, STREET).                |
| `JURIS_DESC`        | object        | Agency responsible for the jurisdiction (usually NYPD).                             |
| `JURISDICTION_CODE` | float64       | Numeric code for the jurisdiction.                                                  |
| `PARKS_NM`          | object        | Name of the NYC park if incident occurred within park boundaries.                   |
| `HADEVELOPT`        | object        | Name of the NYC Housing Authority development, if applicable.                       |
| `HOUSING_PSA`       | object        | Public Service Area code for NYCHA developments.                                    |
| `X_COORD_CD`        | float64       | X coordinate (easting) of the crime location (NYC spatial reference).               |
| `Y_COORD_CD`        | float64       | Y coordinate (northing) of the crime location (NYC spatial reference).              |
| `SUSP_AGE_GROUP`    | object        | Age group of the suspect (e.g., `<18`, `18-24`, `25-44`, `45-64`, `65+`).           |
| `SUSP_RACE`         | object        | Race of the suspect.                                                                |
| `SUSP_SEX`          | object        | Gender of the suspect.                                                              |
| `TRANSIT_DISTRICT`  | float64       | Code of the Transit District (if crime occurred in transit system).                 |
| `Latitude`          | float64       | Latitude coordinate of the crime location.                                          |
| `Longitude`         | float64       | Longitude coordinate of the crime location.                                         |
| `Lat_Lon`           | object        | Combined latitude and longitude field.                                              |
| `PATROL_BORO`       | object        | NYPD patrol borough responsible for policing the area.                              |
| `STATION_NAME`      | object        | Name of the transit station if crime occurred there.                                |
| `VIC_AGE_GROUP`     | object        | Age group of the victim.                                                            |
| `VIC_RACE`          | object        | Race of the victim.                                                                 |
| `VIC_SEX`           | object        | Gender of the victim.                                                               |


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
**Best Location:** Southern Brooklyn and Eastern Queens have less crimes rates.  




