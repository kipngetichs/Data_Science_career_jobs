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


SELECT *COUNT* (*)AS NUMBER_OF_ROWS


FROM DATA_SCIENCE_CAREER_JOBS
 
 
 ![ROW QUALITY CHECK](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/617f7218-0043-422f-9186-3742f3fec27d)
# Column quality check
  SQL QUERY



SELECT COUNT(*)AS COLUMN_COUNT_CHECK

FROM INFORMATION_SCHEMA.COLUMNS

WHERE TABLE_NAME='DATA_SCIENCE_CAREER_JOBS'



![COLUMN QUALITY CHECK](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/981312c9-6926-47f3-9f6d-35a25e1fc968)

  
# Data type check

SQL query



SELECT COLUMN_NAME,DATA_TYPE

FROM INFORMATION_SCHEMA.COLUMNS

WHERE TABLE_NAME='DATA_SCIENCE_CAREER_JOBS'


Output

![DATA TYPE QUALITY CHECK IMG](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/b5e2fe5d-6834-4514-b2ad-5e084a0f15de)

# Null count check

SQL query


SELECT Job_Title,COUNT(*)Null_Count

FROM DATA_SCIENCE_CAREER_JOBS

WHERE    Job_Title IS NULL

GROUP BY   Job_Title


Output

![Null count chech](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/656c6eab-bee5-429c-8344-fe5cf9a15df7)




- The rest of the columns had no null vales i had cross check all

# Column Salaries Where there is 0 salary value.


SQL query



 
SELECT avg_salary,COUNT(*)Zero_Value

FROM DATA_SCIENCE_CAREER_JOBS

WHERE    avg_salary =0

GROUP BY   avg_salary


Output


![Zero value](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/24571d84-9493-477e-b8c7-cc83ecb83519)



- The other min and max salary column didn't have any zero value.
# Visualization


Results

-This is the look of dashboard.

![Dashboard home page img](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/66c8748c-0b1a-421a-84b5-64963736d03b)

![overview dashboard img](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/36ba50b4-1911-4efe-8d9f-ade63023f22a)

# DAX Measures
# 1. Maximum Salary(K)
Maximun Salary(K) = 

var maximun=MAX(Data_Science_Jobss[Maximum_Salary])

RETURN maximun
# 2. Minimum Salary(K)
Minimun Salary(K) = 

var minimun=Min(Data_Science_Jobss[Minimum_Salary])

RETURN minimun
# 3. Average Salary(K)
Average Salary(K) = 

var averagesalary=AVERAGE(Data_Science_Jobss[Average_Salary])

RETURN averagesalary

# Analysis

# Findings

For this analysis,the following are what we need to find out
1. Top 10 sectors with highest salaries distributions
2. Top 5 job titles with highest salary contributions
3. Bottom  5 job titles with lowest  salary contributions
4. Top 5 rated industries
5. Top 10 companies with highest salary contributions
6. Ownerships that are best for  working in
# 1. Top 10 Sectors with highest salary distributions.
|Rank|Sector|Maximum Salary(K)
|---------|--------|---------|
|1|Insurance|$306
|2|Information Technology|$289
|3|Business Services| $275
|4|Health Care| $272
|5|Boitech & Pharmaceuticals|$231
|6|Finance|$228
|7|Aerospace & Defence|$211
|8|Education|$208
|9|Retail|$201
|10|Media|$190

# 2.Top 5 job titles with highest salary contributions
|Rank|Job Title|Maximum Salary(K)
|---------|--------|---------|
|1|Director II, Data Science - GRM Actuarial|$306
|2|Principal Machine Learning Scientist|$289
|3|Senior Data Scientist| $275
|4|Data Science Manager| $272
|5|Director II, Data Science - GRS Predictive Analyti|$231

# 3.Bottom 5 job titles with lowest salary contributions
|Rank|Job Title|Maximum Salary(K)
|---------|--------|---------|
|1|Senior Operations Data Analyst, Call Center Operat|$10
|2|Data Scientist|$15
|3|Medical Technologist / Clinical Laboratory Scienti| $15
|4|Medical Lab Scientist| $17
|5|Medical Laboratory Scientist|$18

# 4.Top 5 rated industries
|Rank|Industry|Average Rating
|---------|--------|---------|
|1|Security Services|4.76
|2|Farm Support Services|4.6
|3|Architectural & Engineering Services| 4.45
|4|Metals Brokers| 4.4
|5|Trucking|4.3

# 5. Top 10 companies with highest salary contributions
|Rank|Sector|Maximum Salary(K)
|---------------|-------------------------|---------|
|1|Liberty Mutual Insurance 3.3|$306
|2|Sage Intacct 4.7|$289
|3|Gallup 4.2| $275
|4|Grand Rounds 4.2| $272
|5|The Climate Corporation 3.2|$238
|6|Nektar Therapeutics 3.5|$231
|7|DTCC 3.3|$228
|8|Samsung Research America 3.7|$228
|9|Tapjoy 3.9|$224
|10|BioMarin Pharmaceutical 3.8|$223
# Notes
For this analysis, we'll prioritize analysing with metrics that are important in generating the expected ROI for the project, which are the career job title,sectors,companies,type of ownership wuth the best salaries
 - Maximum Salary
 - Minimum Salary
 - Average Salary
# Validation
# Top Sectors with best salaries

Calculation Breakdown


The Best Career Sector=Salary Expectation
1. Insurance
 - Maximum Salary(K) = $306
 - Minimum Salary(K)=$32
 - Average Salary(K)=$105.94
2. Information Technology
  - Maximum Salary(K) =$289
  - Minimum Salary(K)=$20
  - Average Salary(K)=$111.94
3. Business Services
  - Maximum Salary(K)=$275
  - Minimum Salary(K)=$15
  - Average Salary(K)=$97.7


   # SQL query for this :
  
   
   select top 3 Sector,

max(Maximum_Salary)Maximum_Salary,

round(avg(Average_Salary),2)Average_Salary,

min(Minimum_Salary)Minimum_Salary

from Data_Science_Jobss

group by Sector

order by Maximum_Salary desc


OUTPUT



![Best Sectors img](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/c0593560-ecd1-43c6-8537-0d65503317a4)

# Top Job Titles With Best Salaries
Calculation Breakdown

Best career job=Salary Expectation


1. Director II, Data Science - GRM Actuarial
    - Maximum Salary = $306
    - Minimun Salary=$202
    - Average Salary=$254

2. Principal Machine Learning Scientist
    - Maximun Salary=$289
    - Minimum Salary=$176
    - Average Salary=$232.5

3. Senior Data Scientist
    - Maximum Salary=$275
   - Minimum Salary=$73
   - Average Salary=$134.87

4. Data Science Manager
   - Maximum Salary=$272
   - Minimum Salary=$95
   - Average Salary=$158.83

5. Director II, Data Science - GRS Predictive Analyti
   - Maximum Salary =$239
   - Minimum Salary=$150
   - Average Salary=$194.5


# SQL query for this :


select top 5 Job_Title,

max(Maximum_Salary)Maximum_Salary,

round(avg(Average_Salary),2)Average_Salary,

min(Minimum_Salary)Minimum_Salary

from Data_Science_Jobss

group by Job_Title

order by Maximum_Salary desc








OUTPUT

  ![Job titles with best salaries img](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/c0f889b2-9d94-44da-b80e-647f14fb8fbd)


# Top Industries With Best Salaries And Ratings
Calculation Breakdown

Career Industry=Salary expectation & Rating

1. Insurance Carriers
   - Maximum Salary(K)=$306
   - Minimum Salary(K)=$32
   - Average Salary(K)=$105.63
   - Average Rating=$3.53
2. Computer Hardware & Software
    - Maximum Salary(K)=$289
    - Minimum Salary(K)=$34
    - Average Salary(K)=$115.19
    - Average Rating=4.05
3. Consulting
   - Maximum Salary(K)=$275
   - Minimum Salary(K)=$37
   - Average Salary(K)=$108.69
   - Average Rating=4.04
4. Health Care Services & Hospitals
   - Maximum Salary(K)=$272
   - Minimum Salary(K)=$17
   - Average Salary(K)=$67.62
   - Average Rating=3.5
5. Enterprise Software & Network Solutions
   - Maximum Salary(K)=$238
   - Minimum Salary(K)=$20
   - Average Salary(K)=$115.37
   - Average Rating=3.96
# SQL query for this :

select top 5 Industry,

round(avg(Rating),2)Average_Rating,

max(Maximum_Salary)Maximum_Salary,

round(avg(Average_Salary),2)Average_Salary,

min(Minimum_Salary)Minimum_Salary

from Data_Science_Jobss

group by Industry

order by Maximum_Salary desc


OUTPUT


![top industries with highest payments img](https://github.com/kipngetichs/Data_Science_career_jobs/assets/169267198/e2a04a3f-a2a3-4138-a80a-2a95be560a59)

# Top Companies With Best Salaries And Ratings
Calculation Breakdown

Best Company=Salary Expectation & Average Rating

1. Liberty Mutual Insurance 
   - Maximum Salary(K)=$306
   - Minimum Salary(K)=$37
   - Average Salary(K)=$153.6
   - Average Rating=3.3
2. Sage Intacct
   - Maximum Salary(K)=$289
   - Minimum Salary(K)=$176
   - Average Salary(K)=$232.5
   - Average Rating=4.7
3. Gallup
   - Maximum Salary(K)=$275
   - Minimum Salary(K)=$200
   - Average Salary(K)=$237.5
   - Average Rating=4.2
4. Grand Rounds
   - Maximum Salary(K)=$272
   - Minimum Salary(K)=$171
   - Average Salary(K)=$221.5
   - Average Rating=4.2
5. The Climate Corporation
   - Maximum Salary=$238
   - Minimum Salary=$150
   - Average Salary=$194
   - Average Rating=3.2
# SQL query for this :
select top 5 Company_Name,

round(avg(Rating),2)Average_Rating,

max(Maximum_Salary)Maximum_Salary,

round(avg(Average_Salary),2)Average_Salary,

min(Minimum_Salary)Minimum_Salary

from Data_Science_Jobss

group by Company_Name

order by Maximum_Salary desc

OUTPUT




