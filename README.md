# Trends in Hospital Readmissions in California Counties (2011-2022)

### Project Overview

---

This project sought to explore hospital readmissions in 57 California Counties from 2011 to 2022. The aim of this analysis was to identify counties with high readmissions and its relation to hospital admissions within the population. Insights gained from this analysis can be used to identify counties that require strategies and resources to reduce hospital readmissions. 

<img width="1233" alt="Total HA" src="https://github.com/user-attachments/assets/e5d20fba-d1b0-41da-886a-ee8958f258fb" />

<img width="1234" alt="Total HRR" src="https://github.com/user-attachments/assets/29719fb2-8f01-4d8e-a05e-947fe941e5b1" />

<img width="1116" alt="HR Trend" src="https://github.com/user-attachments/assets/bd096c75-6632-4065-96b2-83ea686d0d5d" />

<img width="1198" alt="Frequency" src="https://github.com/user-attachments/assets/d0afffe9-4618-4cd7-a4c9-ff31c44c8d23" />

<img width="1175" alt="correlation" src="https://github.com/user-attachments/assets/bc67ee26-510b-4741-ae01-6cc053811c97" />


### Data Sources 
---

The dataset used for this analysis is "Hospital Readmission Rates in California.csv" from kaggle datasets containing healthcare utilization, income and population data for California counties between 2011-2022.[Download here](https://www.kaggle.com/datasets/joshhaber/hospital-readmission-rates-in-california )

### Tools
---

- SQL (MySQLWorkbench) - Data Cleaning and Formatting 
- SQL (MySQLWorkbench) - Analysis of Data using SQL queries (Joins, Subqueries, IF function) 
- Power Bi- Data Visualization 

### Data Cleaning/Preparations
---
The following tasks were performed during the data preparation stage 
- Data loading and Inspection 
- Data Cleaning and Formatting

### Data Analysis
---

SQL queries (Joins, Subqueries, IF function)  were used to identify counties with high readmissions rates, frequency of high readmissions as well as trends over the period. Example of SQL queries used were:

``` SELECT A.County, A.Total_adm, B.Total_Readm FROM county_adm AS A INNER JOIN county_readm as B ON A.County= B.County; ```

``` SELECT County, Frequency, IF(Frequency > '5', 'Above','Below') AS Levels FROM freqtrial; ```

  ### Questions
---

1. Which 10 Counties had the highest hospital admissions and their total number of admissions from 2011 to 2022?
2. Which 10 Counties had the highest rate of hospital readmissions and their total readmissions rate from 2011 to 2022?
3. Which counties had both highest total readmission rate and admission?
4. What is the total readmission rate of 10 counties with the highest hospital readmissions during the period of study (2011 to 2022)?
5. What is the frequency of counties with the highest hospital readmissions over the period?
6. What is the total number of counties that contributed to high hospital readmissions?
7. Which counties contributed to high hospital readmissions more than two times?
8. What counties experienced very high readmissions among the 29 high readmission counties (Threshold- Frequency above or below 5)?
9. What counties among the 29 high readmission counties are below the threshold (Threshold- Frequency above or below 5)?
10. What is the Per Capita Personal Income of the counties that had most readmission over the period against the national Per Capita Personal Income?

### Summary of Findings
---

1. The 10 counties with the highest hospital admissions were Los Angeles, San Diego, Orange, Riverside, San Bernardino, Sacramento, Santa Clara, Alameda, Contra Costa and Fresno with admissions ranging from 565,825 to 5,515,350.
2. The 10 counties with the highest rate of hospital readmissions were Butte, Los Angeles, Lake, Alameda, Yuba, Fresno, Merced, San Joaquin, Contra Costa and San Bernadino with total hospital readmission rate ranging from 174.0 to 209.3 (2011- 2022).
3. Counties with both highest readmission rate and total admissions were Los Angeles, Alameda, Fresno, Contra Costa and San Bernardino.
4. The total readmission rate of 10 counties with the highest hospital readmissions during the period of study range from 144.2 in 2015 to 180.1 in 2022.
5. The frequency of counties with the highest hospital readmissions over the period ranged from 1 to 12.
6. The total number of counties that contributed to high hospital readmissions over the period was 29.
7. Counties that contributed to high hospital readmissions more than two times were Butte, Los Angeles, Alameda, Lake, Yuba, San Bernardino, Merced, Fresno, Contra Costa, Imperial, Sacramento, San Joaquin, Napa, Colusa and Glenn.
8. Of the 29 counties that contributed to high hospital readmissions over the period, 9 counties experienced very high readmissions with frequency ranging from 6 to 12.
9. Of the 29 counties that contributed to high hospital readmissions over the period, 20 counties were below the frequency threshold of 5; with frequency ranging from 1 to 4.
10. For counties that had most readmission over the period, some had Per Capita Personal Income above the national Per Capita Personal Income while others were below.

### Recommendations
---

The following actions are recommended based on the analysis: 
- Public Health interventions should be implemented as a proactive measure to curb increase in both hospital admissions and readmissions.
- A study to investigate factors that contribute to hospital readmissions in counties with high readmission is recommended in order to identify strategies and resources required to reduce hospital readmissions.
- A study to investigate the trend of Per Capita Personal Income in counties and the extent of its influence on both hospital admissions and readmissions is recommended.

### Limitations 
---

Information on 1 County of California (San Francisco) was not available at the time of analysis and could not be included in the analysis.  

### References 
---

1. Haber, J. (2021). Hospital Readmission Rates in California. Kaggle. Available at: https://www.kaggle.com/datasets/joshhaber/hospital-readmission-rates-in-california
2. Bureau of Economic Analysis (BEA). (2012). Local Area Personal Income: 2009-2011. Available at: https://www.bea.gov/index.php/news/2012/local-area-personal-income-2009-2011
3. Bureau of Economic Analysis (BEA). (2016). Local Area Personal Income: 2015. Available at: https://apps.bea.gov/scb/pdf/2016/12%20December/1216_local_area_personal_income.pdf?_gl=1*1pvgg35*_ga*MjA3NjA3NDUyMS4xNzQwNTk0NjM4*_ga_J4698JNNFT*MTc0MDY0Njg4NC41LjEuMTc0MDY0NzIwNS44LjAuMA.. 
