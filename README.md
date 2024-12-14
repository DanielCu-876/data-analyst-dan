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
