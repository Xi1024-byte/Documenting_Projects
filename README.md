# Healthcare Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Recommendations](#recommendations)

## Project Overview
This healthcare data analysis project aims to gain insights into patient health conditions, medical encounters, immunizations, and patient demographics. By analyzing these datasets, we seek to understand trends, identify correlations, and make data-driven recommendations to improve healthcare services and patient outcomes.

## Data Sources
- **Patients Data**: Contains demographic information about patients, including birthdate, deathdate, social security number (SSN), driver's license number, passport number, name prefixes, first name, last name, name suffixes, maiden name, marital status, race, ethnicity, gender, and birthplace.
- **Conditions Table**: Contains information about health conditions diagnosed in patients, including start and stop dates, patient ID, encounter ID, condition codes, and descriptions.
- **Encounters Table**: Provides details about medical encounters, including encounter ID, start and stop timestamps, patient ID, organization, provider, payer information, encounter class, encounter codes, encounter descriptions, encounter costs, total claim costs, payer coverage, and reason codes.
- **Immunizations Table**: Records immunizations administered to patients, including dates, patient ID, encounter ID, immunization codes, and descriptions.
  
### Tools
- Excel - Data Cleaning
  - [Download here](https://www.microsoft.com/en-gb/microsoft-365/excel?ef_id=_k_Cj0KCQjw8J6wBhDXARIsAPo7QA8nXS_ysCK_668DYB5T2daBnpg6jIdmkI6VLwBY1lQPiqNEzDUVvrQaAo57EALw_wcB_k_&OCID=AIDcmmp20rgnjr_SEM__k_Cj0KCQjw8J6wBhDXARIsAPo7QA8nXS_ysCK_668DYB5T2daBnpg6jIdmkI6VLwBY1lQPiqNEzDUVvrQaAo57EALw_wcB_k_&gad_source=1&gclid=Cj0KCQjw8J6wBhDXARIsAPo7QA8nXS_ysCK_668DYB5T2daBnpg6jIdmkI6VLwBY1lQPiqNEzDUVvrQaAo57EALw_wcB)
- PostgreSQL -Data Analysis
- Tableau -Creating visual reports and dashboards


#### Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks:
1. Loading and inspection of data from various sources.
2. Handling missing values and data inconsistencies.
3. Data cleaning and formatting.

#### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions, such as:
  - What is the distribution of different health conditions among patients?
  - What is the valuation of encounter costs and insurance coverage?
  - What are the trends in immunization rates over time?
  - Which are the most frequently administered vaccines?
  - What is the tribution of patients by age, gender, race, and ethnicity?

#### Data Analysis
Include some interesting code/features worked with

```SQL
SELECT *
FROM patients
WHERE age > 55 and gender = 'F';
```

#### Results/Findings
The analysis results are summarized as follows:
1. The most prevalent health conditions among patients are [______]
2. Patients with [____specific conditions_ _] have higher encounter costs and lower insurance coverage.
3. Immunization rates have shown a [  _e.g._steady increase__] over the past [ ___ time period__ ].
4. The [ __ specific vaccine__  ] is the most commonly administered immunization, followed by [ __others__ ].
5. The patient population is predominantly [ _ _demographic characteristic__  ].

## Recommendations
Based on the analysis, we recommend the following actions:

  - Enhance Preventive Healthcare Programs
  - Invest in Healthcare Infrastructure
  - Targeted Health Education Campaigns
  - Identify and Ensure adequate supply and distribution of administered vaccines 
  - Implement Patient Engagement Strategies to target healthcare providers effectively


### Limitations
I had to remove all zero values from budget and revenue columns because they would have affected the accuracy of my conclusions from the analysis. There are still a few outliers even after the omissions but even then we can still see that there is a positive correlation between both patients and number of vaccines.

### References
1.[Youtube _ How to Document Data Analysis Projects on GitHub](https://www.youtube.com/watch?v=0N9xekdKCwk)

2.Data Sources
  [1](https://click.convertkit-mail2.com/mvun2m3eomsps6kl2tmhe9m7lqq/25h2hoh20w4g2ot3/aHR0cHM6Ly9kb3dubG9hZC5maWxla2l0Y2RuLmNvbS9kL2ttRDNDcWVMTkZXTmltV0Z1R014bXQvNkwyUWRhUExUMndWYlZqYkxhWEhaVw==)
  [2](https://www.dropbox.com/scl/fi/914gq2qrej6enwwaoc5vp/encounters.txt?rlkey=uwc55hnx2d16kmcuvvampefkb&dl=0https://www.dropbox.com/scl/fi/914gq2qrej6enwwaoc5vp/encounters.txt?rlkey=uwc55hnx2d16kmcuvvampefkb&dl=0)
