# HR-Analytics


## Table Of Contents

- [Project Overview](#project-overview)
- [Audience](#audience)
- [Data Sources](#data-sources)
- [Data Structure](#data-structure)
- [Tool used for the analysis](#tool-used-for-the-analysis)
- [Data Preparation](#data-preparation)
- [Creating a Date Table Using DAX](#creating-a-date-table-using-dax)
- [Data Modelling](#data-modelling)

 
## Project Overview 

This project is an end-to-end HR analytics solution built on Microsoft Fabric, designed to transform raw HR data into actionable insights. The solution begins with a structured pipeline where Dataflow Gen2 is used to collect, clean, and transform datasets from multiple HR source systems, ensuring consistency and reliability. The processed data is then stored in a Fabric Lakehouse, which serves as a scalable single source of truth, while a Semantic Model was developed to support dynamic analysis and real-time reporting. To deliver insights, a Power BI dashboard was created and directly integrated with the Semantic Model, enabling leadership to explore attrition drivers, predictive risk scores, and workforce trends in an interactive and intuitive way. The entire ETL and reporting process was orchestrated and automated using Fabric Pipelines, ensuring data freshness and minimizing manual intervention. Designed with scalability and reusability in mind, this system is well-prepared for real-world deployment in HR tech environments, demonstrating how Microsoft Fabric can enable organizations to drive data-informed workforce decisions.


<img width="1351" height="726" alt="Screenshot 2025-07-15 192124" src="https://github.com/user-attachments/assets/48b1caa2-94a9-47ba-9f50-c9cadad336d1" />

<img width="1335" height="718" alt="Screenshot 2025-07-15 200734" src="https://github.com/user-attachments/assets/e2c36120-caee-4c53-9a22-23d85c48aae6" />

[Dashboard Link](https://app.fabric.microsoft.com/links/-x1TUBp104?ctid=6d461a65-c4ee-4ee1-a98c-4188e8a1219d&pbi_source=linkShare)

## Audience 

-Executive
-HR Managers

## Data Sources 

- "education_levels.csv" : contains detailed information employee education levels 
- "employee.csv" : details of employees
- "performance.csv" : information about employees performance
- "rating.csv": details of employee ratings"
- "satisfaction.csv" : information about employee satisfaction

## Data Structure
- Multiple Tables: 5
- Number of Records: 
- Number of Fields: 22
  
## Tool used for the analysis 
Microsoft  Fabric & PowerBI- for cleaning, analyzing and building reports. 

## Data Preparation 

The data was mostly clean,so there was not much cleaning required. However, the following steps were taken to ensure data validity:
1. Data loading and inspection
2. Changed type of some columns
3. Removed unnecessary columns
4. Handled missing values: There were about 15% missing valus in the patient location data, but these missing values did not significantly affect the analysis, so they were left as it was.
5. Created a date table using Dax to facilitate time-based analysis.

