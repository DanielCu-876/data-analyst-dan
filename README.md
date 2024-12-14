# data-analyst-dan

Project 1 

Project Description :

    Analyzing the workforce to determine the number of males employed.

Project Title :

    Workforce Gender Distribution Analysis

Objective
    
    The calculate and describe the number of males employed in the workforce.

Dataset

    Year: The calendar year of the data (e.g., 2023).
    Exempt/Union: Indicates whether the employee belongs to a union or is exempt from it.
    Classification: Job classification, including grouped or individual roles.
    Position Title: The title of the position, which may be specific or aggregated across multiple roles.
    Data Category: Specifies whether the data is detailed for an individual role or aggregated across multiple roles.
    Minimum Hourly Rate: The minimum hourly wage for a role (if applicable).
    Maximum Hourly Rate: The maximum hourly wage for a role (if applicable).
    Female: Number of female employees in the given job classification.
    Male: Number of male employees in the given job classification.
    Total: Total number of employees in the given job classification (sum of male and female employees).

This dataset provides detailed information on workforce demographics, salary ranges, and job roles, enabling descriptive analysis of employment trends, gender distribution, and pay equity.

Methodology


Data Collection and Preparation:

![image](https://github.com/user-attachments/assets/8ea19b4d-75fa-440e-a3d1-a5e5b7803c5e)

    Load the dataset into AWS using data ingestion methods.
    Perform data cleaning to address missing values, correct data types, and remove duplicates.



Descriptive Statistics:

    Calculate the total number of males employed across all job classifications.

Data Visualization:

    Use bar charts or pie charts to represent gender distribution in the workforce.

Customer Segmentation:

    Segment by job classification, department, or pay rates if relevant to the analysis.

Insights and Findings:

    Summarize key insights, such as the proportion of male employees relative to the total workforce and distribution trends across classifications.

Recommendations:

    Provide actionable recommendations based on gender distribution data to address workforce diversity goals or resource planning.

Tools and Technologies 

    AWS S3, DataBrew, DataGLue.

Deleverables

    A report summarizing the findings, visualizations of gender distribution, and actionable recommendations.



Project 2 

Project Description:
    
    Exploring the workforce dataset to identify how many positions have a maximum hourly rate that is at least double the current minimum wage in British Columbia, which is $17.40.

Project Title:
    
    Analysis of Positions with High Maximum Hourly Rates

Objective:
    
    To determine the number of positions with a maximum hourly rate of at least $34.80 (twice the minimum wage in British Columbia).

Dataset

    Year: The calendar year of the data (e.g., 2023).
    Exempt/Union: Indicates whether the employee belongs to a union or is exempt from it.
    Classification: Job classification, including grouped or individual roles.
    Position Title: The title of the position, which may be specific or aggregated across multiple roles.
    Data Category: Specifies whether the data is detailed for an individual role or aggregated across multiple roles.
    Minimum Hourly Rate: The minimum hourly wage for a role (if applicable).
    Maximum Hourly Rate: The maximum hourly wage for a role (if applicable).
    Female: Number of female employees in the given job classification.
    Male: Number of male employees in the given job classification.
    Total: Total number of employees in the given job classification (sum of male and female employees).

Methodology:

    Data Collection and Preparation:
        Use an ETL pipeline to extract, transform, and load data into a structured format.
        Store the dataset in AWS S3 for scalable storage.
        Query and analyze the dataset using AWS Athena to handle large-scale computations.

    Data Analysis Process:
        Query the dataset in Athena to identify rows where the "Maximum hourly rate" is at least $34.80.
        Count the number of unique positions meeting this condition.
        Perform data validation checks to ensure accuracy.

    Exploratory Statistics and Visualization:
        Summarize the dataset using aggregate queries in Athena.
    
Tools and Technologies:

        ETL Pipeline: Extract, Transform, Load process.
        AWS S3: For secure and scalable data storage.
        AWS Athena: For querying and analysis.

Deliverables:

    A summarized report with the number of positions that meet the criterion.
    Visualizations to represent the distribution of positions by maximum hourly rate.
    Recommendations for further analysis or policy adjustments based on findings.

Project 3

    Implementation of Data Quality Control Measures at UCW within the Human Resources department, specifically the disciplinary actions comitee. 

Project Description:

    Data Quality Control Initiative within UCW Human Resources department's disciplinary comitee

Project Title:

    Implementation of Data Quality Control Measures within UCW’s Disciplinary Actions Committee

Objective:
    
    The primary objective of this project is to establish a robust Data Quality Control (DQC) framework tailored to the Human Resources department, specifically addressing the Disciplinary Actions Committee’s data. This initiative aims to enhance the accuracy, completeness, and consistency of disciplinary records, ensuring compliance with internal policies, regulatory requirements, and enabling data-driven decision-making.

Scope:

The project will focus on the following key areas:

    Data Profiling: Evaluating existing disciplinary records to assess quality and identify key issues.
    Data Cleansing: Developing processes to correct inaccuracies, remove duplicates, and address inconsistencies.
    Data Validation: Setting validation rules to ensure integrity for both historical and new disciplinary action records.
    Monitoring and Reporting: Creating dashboards to track data quality metrics for HR operations.

Methodology:

    Current State Assessment:
        Review existing disciplinary action records and workflows within the HR department.
        Identify key issues such as incomplete records, duplicate entries, and inconsistent data formatting.

    Data Profiling:
        Use AWS Glue DataBrew to profile datasets, assessing completeness, accuracy, validity, and consistency.
        Highlight critical gaps in key data fields such as case identifiers, dates, and employee details.

    Establish Data Quality Metrics:
        Define and track metrics, including:
            Error rates (e.g., incorrect case information).
            Record duplication levels.
            Timeliness of data entry and updates.
        Set baseline KPIs for ongoing improvements.

    Data Cleansing Processes:
        Use AWS Glue DataBrew to:
            Remove duplicate or redundant records.
            Correct errors in case details (e.g., misclassified actions or incomplete employee information).
            Standardize data formats, particularly for dates, names, and action classifications.

    Validation Rules and Procedures:
        Create automated validation checks for new disciplinary records using AWS Glue DataBrew's validation features.
        Define standard operating procedures for data entry to ensure consistency.

    Monitoring and Reporting:
        Store cleansed data in AWS S3 for future integration with Tableau or Power BI for visualization.
        Develop real-time dashboards to monitor data quality metrics.
        Automate periodic reporting to identify trends and highlight deviations from quality standards.

    Training and Best Practices:
        Provide training sessions to HR staff on data handling and the importance of quality assurance.
        Distribute user-friendly guidelines to ensure adherence to best practices in record-keeping.

    Feedback Mechanism:
        Establish a feedback loop for continuous improvement, enabling committee members to report data quality issues and suggest enhancements.

Tools and Technologies:

    Data Profiling and Cleansing: AWS Glue DataBrew for profiling, cleaning, and validation tasks.
    Data Storage and Processing: AWS S3 for scalable data storage.
    Visualization Tools: Tableau or Power BI for dashboards.
    Automation Scripts: Python and SQL for additional data transformations if needed.

Deliverables:

    A Data Quality Control plan tailored to the Disciplinary Actions Committee’s needs.
    Documented metrics and KPIs for monitoring data quality.
    A cleaned and standardized dataset of disciplinary actions stored in AWS S3.
    Training materials and sessions for HR staff and committee members.
    Dashboards to visualize data quality metrics and trends.

Timeline:

    Weeks 1–2: Current state assessment and data profiling of disciplinary action records.
    Weeks 3–4: Develop and implement data cleansing processes using AWS Glue DataBrew.
    Weeks 5–6: Establish validation rules and deploy monitoring dashboards.
    Weeks 7–8: Conduct staff training and finalize a feedback mechanism.
