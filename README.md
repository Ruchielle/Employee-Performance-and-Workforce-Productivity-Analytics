## Employee Performance and Workforce Productivity Analytics

### Project overview 

The Employee Performance and Workforce Productivity Analytics Dashboard is a Power BI project developed to analyze employee performance, workforce productivity, compensation, attendance, and career progression.
The dataset contains 5,000 employee records across 11 fields, covering employee demographics, department, job level, salary, years at the company, performance score, promotion history, absence days, and work mode.
The analysis was tailored to provide a clearer view of workforce performance and help identify patterns across employee performance, compensation, attendance, career growth, age, department, and work mode.
Using Power Query, DAX, and Power BI, the project transformed the employee dataset into an interactive dashboard consisting of three analytical pages
 - Attendance Overview
 - Performance and Pay Overview
 - Demographics and Career Overview 
The dashboard provides an interactive way to examine employee performance, salary patterns, absence levels, promotions, and workforce characteristics across different employee groups.


### Project Objectives 

 - Understand workforce demographics, clearly breaking down employee details like age, department, job level, tenure, and work setup. 
 - Monitor daily habits and presence, looking closely at attendance, absences, and how different work modes affect daily routines.
 - Measure performance across teams, easily comparing productivity levels across different departments and work setups.
 - Compare pay and promotions with performance, evaluating how employee salary and promotions directly relate to performance.
 - Discover  career growth and promotion trends, tracking how team members advance over time and across different employee groups.
 - Bring it all together in an interactive dashboard, giving users a central place to explore and interact with all these workforce insights.

### Tools

 - Power BI

Used for:

   - Dashboard development
   - Interactive visualization
   - KPI presentation
   - Filtering and exploration

 - Power Query

Used for:

   - Data validation
   - Data quality checks
   - Missing value checks
   - Column quality review
   - Promotion date consistency checks
   - Text consistency checks
   - Data transformation

 - DAX

Used for:

   - Creating analytical measures
   - Calculating employee and promotion metrics
   - Calculating promotion rate
   - Calculating average salary
   - Calculating average performance
   - Creating analytical categories and groups


### Data Workflow

 - Source 
     - This project is built using an employee performance dataset sourced from Kaggle, containing 5,000 employee records and 11 columns. The dataset provides a comprehensive look into workforce dynamics, covering key areas such as demographics, compensation, performance, promotions, attendance, and work arrangements.

 - Dataset Fields
    
    - Employee ID: A unique identifier assigned to each employee.
    
    - Age: The current age of the employee.
    
    - Gender: The gender identity of the employee.
    
    - Department: The organizational department the employee belongs to.
    
    - Job Level: The employee's current role hierarchy or tier.
    
    - Salary: The compensation or pay rate for the employee.
    
    - Years at Company: The total duration of time the employee has spent with the organization.
    
    - Performance Score: The evaluated metric representing the employee's work output and effectiveness.
    
    - Promotion Date: The historical date associated with the employee's last promotion.
    
    - Absence Days: The total number of days the employee was absent from work.
    
    - Work Mode: The employee's designated work arrangement (e.g., remote, hybrid, or on-site).


 - Ingestion
      - The employee dataset was imported into Power BI to serve as the foundation for data transformation, analysis, and dashboard development. Before building the final analytical model, the raw data underwent a thorough review and initial profiling process using Power Query.

 - Cleaning
      - The data was imported into Power Query to make sure there were no errors. I checked the column quality, making sure that the data types were correct. I checked for missing values, fixed the text to make sure the fields were written correctly, checked for dates to make sure the formats were right, and reviewed the structure to make sure all fields were set up properly.

 - Transformation
      - The data was transformed to support workforce analysis by creating new groups and categories. I created age groups, performance categories, job-level categories, and years-at-company groups. I also extracted the promotion year from the promotion dates and renamed Work Location to Work Mode for clearer terminology. Specifically, performance scores were grouped into Low (Score ≤ 2), Average (Score = 3), and High (Score ≥ 4), job levels were grouped into Entry, Mid, and Senior, and years at the company were grouped into ranges from 0 to 20 years.
 
 - Analysis
      - The analysis focused on exploring employee performance, compensation, attendance, promotions, and overall workforce characteristics. I looked closely at the distribution of performance, salary by performance category, performance across different work modes and departments, and employee absence patterns by department. I also examined promotion patterns by age group and year, along with workforce characteristics like age groups, job levels, tenure groups, and gender and department breakdowns.

 - Output
      - The final output was an interactive Power BI dashboard consisting of three pages. The first page was an Attendance Overview focusing on absence patterns, the second was a Performance and Pay Overview focusing on performance, salary, departments, and work modes, and the third was an Demographics and Career Growth page focusing on age groups, promotions, and career progression. The dashboard also includes interactive filters for gender, department, and work mode.


### Key Metrics
 - Total Employees — Measures the total number of employees in the dataset.
 - Promotion Rate % — Measures the proportion of employees associated with promotions.
 - Average Salary — Measures the average employee salary.
 - Average Performance Score — Measures the average employee performance score.
 - Average Absence Days — Measures the average number of absence days.


### Data Cleaning and Transformation
 - Column Review 
    - The dataset was reviewed to understand the structure and relevance of each field before analysis.
 
 - The original dataset contained 11 columns:
    - Employee ID,
Age,
Gender,
Department,
Job Level,
Salary,
Years at Company,
Performance Score,
Promotion Date,
Absence Days,
Work Location,
The Work Location field was later renamed Work Mode.
 

 - Renamed Columns
     - Work Location to Work Mode
The field originally identified as Work Location was renamed to Work Mode to provide clearer terminology for the employee work arrangement categories.

 - Handled Missing Values
     - The dataset was reviewed for missing values during the Power Query data quality process.
     - The data was checked to make sure there were no missing records affecting the analysis.
 
 - Duplicate Check
     - A data quality review was performed as part of the preparation process.
The dataset was checked for duplicate entries to ensure data integrity.
 
 - Data Type Corrections
     - Data types were reviewed during the Power Query preparation process to ensure correct formatting.
     - The project specifically required validation of fields such as:
 Promotion Date,
 Age,
 Salary,
 Years at Company,
 Performance Score,
 Absence Days, 
 Invalid Values,
 The dataset was reviewed for data quality and consistency issues.
 Text consistency and promotion date consistency were specifically reviewed during the preparation process to ensure all fields were written and formatted correctly.
 
 - Calculated Columns and Analytical Fields
The following analytical fields were created to support the dashboard:
 
     - Performance Category: Classifies employees based on Performance Score:
          - Low: ≤ 2
          - Average: 3
          - High: ≥ 4
 
     - Job Level Category: Groups job levels into distinct categories based on their numerical ranking:
          - Entry: Level 1
          - Mid: Level 2
          - Senior: Level 3

 
     - Years Group: Groups employee servive year at the into ranges:
          - 0–5
          - 6–10
          - 11–15
          - 16–20 years
 
     - Promotion Year: Extracts the year from Promotion Date to support analysis of promotion trends over time.

### Key Analytical Insights
 - Absence by Work Mode
    - Hybrid employees had the highest average absence at 7.64 days.
    - Remote employees followed closely at 7.63 days.
    - In-Office employees had the lowest average at 7.30 days.
    - Insight: The difference is small, meaning work mode does not appear to have a strong relationship with absence in this dataset.

 - Absence vs. Performance
    - High-performing employees averaged 7.56 absence days.
    - Average performers averaged 7.52 absence days.
    - Low performers averaged 7.48 absence days.
    - Insight: This suggests that absence and performance have almost no relationship in this dataset.
 
 - Absence by Gender
     - Average absence across gender groups:
     - Female: 7.57 days
     - Male: 7.54 days
     - Non-binary: 7.45 days
     - Insight: The differences are very small and do not indicate a meaningful gap between the groups.
 
 - Promotion Trend
      - Promotion activity remained fairly stable from 2020 to 2024, with approximately 950–1,000 promotions each year.
      - The 2025 value was much lower, but this is because 2025 represents a partial year in the dataset and should not be treated as evidence of a decline.
 
 - Absence by Department
      - Marketing recorded the highest average absence at 7.57 days.
      - HR recorded the lowest average absence at 7.41 days.
      - Insight: The difference is small, showing that absence is generally consistent across departments.

