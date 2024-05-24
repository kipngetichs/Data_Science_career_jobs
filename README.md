# DATA SCIENCE BEST CAREER JOBS CHOICE PORTFOLIO
![pexels-pixabay-265087](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/9cc74598-c638-4200-880c-a2cd6c6fa347)

## Table of Contents
  - Objective 
- Data Source
- Stages
- Design
  - Mockup
   - Tools
- Development
   - Pseudocode
   - Data Exploration
   - Data Cleaning
   - Transform the Data
   - Create the SQL View
- Testing
  - Data Quality Tests
- Visualization
  - Results
  - DAX Measures
-  Analysis
    - Findings
     - Validation
    - Discovery
 - Recommendations
    - Potential ROI
    -  Potential Courses of Actions 
 - Conclusion
## Objective
- Key Point 




The  key objective of this  project is to provide a comprehensive overview of salary distributions across various sectors and industries. By analyzing key metrics such as maximum salary, minimum salary, and average salary for each sector, industry,type of ownership,size and company, this report aims to identify trends, disparities, and potential areas for improvement .
- Ideal Solution



To create a dashboard that provides insights into the DATA SCIENCE BEST CAREER JOBS CHOICE  that includes their
- Maximum Salary
- Mininum Salary
- Average Salary

This will helps us to know which is the best jobs,sectors,companies and tpye of onwership to work in data science space interms of salary expectations and also poorest areas which needs improvement.
# Data Source
- The data needed to achieve our objective.



Data needed is Glassdoor_Salary_Cleaned_Version that includes their:
- Salary Estimate
- Rating
- Company Name
- Location
- Headquarters
-  Size
- Type Of Ownership
- Industry
- Sector
- Minimum Salary
- Average Salary
- Maximum Salary
- Company Text
 - Job State
 - The data is sourced from Kaggle (an Excel extract),https://www.kaggle.com/datasets/nadzmiagthomas/australia-data-science-jobs
 # Stages
  - Design
 - Developement
- Testing
- Analysis
# Design
# Dashboard Components Requirement
The following are  questions that the dashboard will answer.
- Top 10 Sectors with highest salaries
- Top 5 job titles with highest salaries
- Bottom 5 job titles with lowest salaries
- Average salaries in diffirent locations and job states
- Top 5 rated industries
- Top 10 Companies with highest salaries
- Grid showing all the contents i.e total job titles,companies etc



For now, these are some of the questions we need to answer, this may change as we progress down our analysis
# Dashboard Mockup
Some of the data visuals that may be appropriate in answering our questions include:
1. Table
2. Horizontal bar chats
3. Map
4. Donat Chat
5. Column Bar Chats

![Home Page_1716379105226696](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/94e11a2c-1af0-46d7-97c6-91af5e69fb6f)
![Summary_1716379106121111](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/6816ae54-6b92-44ec-99ef-8220565bc426)
# Tools
| Tool | Purpose |        
|------------|------------|
| Excel | Exploring the data | 
| SQL Server  | Cleaning, testing, and analyzing the data    | 
| Power BI  | Visualizing the data via interactive dashboards  | 
| GitHub  | 	Hosting the project documentation and version control  | 
| Mokkup AI   | 	Designing the wireframe/mockup of the dashboard  | 
# Development

# Pseudocode
  - The general approach in creating this solution from start to finish was:
 1. Get the data
 2. Explore the data in Excel
 3. Load the data into SQL Server
 4. Clean the data with SQL
 5. Test the data with SQL
 6. Visualize the data in Power BI
 7. Generate the findings based on the insights
 8. Write the documentation + commentary
 9. Publish the data to GitHub Pages
# Data exploration notes
- The Following was my initial observation that caught my Attention:


  1. Salary Analysis: The columns related to salary (min_salary, max_salary, avg_salary) provide a comprehensive view of compensation. The data can be explored to identify trends in salary by job title, location, industry,sectors,type of ownership,companies and company size.
  2. Company Attributes: Information about the company (size,  type_of_ownership, industry, sector, ) allows for a detailed analysis of how company characteristics correlate with job offerings and salaries.
  3. Geographic Distribution: Location and job_state provide the basis for geographic analysis, helping to understand where jobs are concentrated and how location impacts salary and job availability.
  4. Reputation : Rating column can be used to evaluate company reputation and  positioning we can be able to see characterictisc of different (sectors,companies,type of ownerships and industries)
  5. Skill Demand: Columns like python_yn, R_yn, spark, aws, and excel offer insights into the technical skills demanded by employers. This can be analyzed to identify the most sought-after skills in the job market.
  # Data cleaning
 - Expectations to the data.
 
  The aim is to refine our dataset to ensure it is structured and ready for analysis.
  
  The cleaned data should meet the following criteria and constraints:
  - Only relevant columns should be retained.
  - All data types should be appropriate for the contents of each column.
  - No column should contain null values, indicating complete data for all records.
  - Columns like(min_salary,max_salary,avg_salary)should not contain 0 values for it will not make any sense at all.

Below is a table outlining the constraints on our cleaned dataset:

| Property| Description |        
|------------|------------|
| Number of Rows| 731 | 
| Number of Columns  |20    | 

And here is a tabular representation of the expected schema for the clean data:
| Column Name| Data Type|   Nullable     |
|------------|------------|--------|
| Job_Title| VARCHAR|     NO  |
|Rating|FLOAT|NO     
|Company_Name| VARCHAR|NO
|Location|VARCHAR|NO
|Headquarters|VARCHAR|NO
|Size|VARCHAR|NO
|Type_of_ownership|VARCHAR|NO
|Industry|VARCHAR|NO    
|min_salary|INTEGER|NO    
|max_salary| INTEGER|NO 
|avg_salary|FLOAT|NO
|company_txt|VARCHAR|NO
|job_state|VARCHAR|NO
|python_yn|BINARY|NO
|R_yn|BINARY|NO
|spark|BINARY|NO
|aws|BINARY|NO
|excel|BINARY|NO

# Transform the data
SQL QUERY


![Transform img sql](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/11349aa7-2ae2-43c7-a16e-6d0a6d7179f9)

# Create the SQL view
 SQL QUERY


![SQL VIEW](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/f02a605e-51f5-4883-bcfa-f990d5a22404)
# Testing
Here are the data quality tests conducted:
# Row count check
 SQL QUERY





