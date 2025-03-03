# Trends in Hospital Readmissions Across California Counties (2011-2022)

### Project Overview

---

This project sought to explore hospital readmissions in 57 California Counties from 2011 to 2022. The aim of this analysis was to identify counties with high readmissions and its relation to hospital admissions within the population. Insights gained from this analysis can be used to identify counties that require strategies and resources to reduce hospital readmissions. 

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


