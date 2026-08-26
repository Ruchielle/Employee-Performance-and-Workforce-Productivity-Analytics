## Employee Performance and Workforce Productivity Analytics


## Table of Content 
 - [Projects Overview](#project-overview)
 - [Project Objective](#project-objective)
 - [Tools](#tools) 
 - [Data Workflow](#data-workflow) 
 - [Key Metrics](#key-metrics)
 - [Data Cleaning and Transformation](#data-cleaning-and-transformation)
 - [Exploratory Data Analysis](#eploratory-data-analysis)
 - [Key Insights and Visuals](#key-insights-and-visuals)
 - [Recommendations](#recommendation)
 - [Assumptions](#assumptions)
 - [Limitations](#limitations)
 - [Author](#author)

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



### Exploratory Data Analysis
The exploratory analysis was structured around key business questions related to workforce performance, productivity, and career growth.
 - Workforce Composition
      - How many employees are represented in the dataset?
      - How is the workforce distributed across departments?
      - How is the workforce distributed by gender?
      - How are employees distributed across job levels?
      - How does employee tenure vary across the workforce?

 - Employee Performance
      - How are employees distributed across performance categories?
      - What proportion of employees fall into Low, Average, and High performance categories?
      - How does average performance vary across departments?
      - How does average performance vary across work modes?

 - Performance and Compensation
      - How does average salary vary across performance categories?
      - Are salary patterns different across Low, Average, and High-performing employees?
      - How does salary vary across employee performance groups?

 - Attendance
      - How many absence days are recorded across the workforce?
      - How does average absence vary by department?
      - Which departments show differences in average absence days?

 - Career Growth and Promotions
      - How many employees have recorded promotions?
      - How does promotion activity vary across age groups?
      - How have promotions changed over time?
      - Which age groups show different promotion patterns?


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
      - The 2025 value was much lower because the data stops in February 2025. Therefore, this drop should not be treated as evidence of a decline in promotions.

 - Absence by Department
      - Marketing recorded the highest average absence at 7.57 days.
      - HR recorded the lowest average absence at 7.41 days.
      - Insight: The difference is small, showing that absence is generally consistent across departments.

 - Workforce by Performance Category
     - High Performance: 2,000 employees
     - Low Performance: 2,000 employees
     - Average Performance: 1,000 employees
     - Insight: This shows a highly divided performance distribution, with more employees at the High and Low ends than in the Average category. This may be worth reviewing to determine whether managers are using the full performance rating scale consistently.

 - Performance by Gender
     - Average performance scores were almost identical across groups:
     - Male: 3.01
     - Non-binary: 3.01
     - Female: 3.00
     - Insight: There is no meaningful performance difference between the groups in this dataset.
 
 - Promotions by Years at Company
     - Employees with 6–10 years and 16–20 years at the company recorded the highest number of promotions.
     - Insight: However, the differences between tenure groups were relatively small, suggesting that years at the company alone is not the main factor determining promotion.
 
 - Performance by Department
      - The highest-performing departments were:
      - Sales: 3.03
      - Engineering: 3.03
      - HR: 3.02
      - Marketing: Recorded the lowest average performance score at 2.95.
      - Insight: This could encourage HR to investigate whether Marketing needs additional training, workload adjustments, or management support.

 - Salary vs. Performance
      - One of the most important findings was that average salary remained almost the same across High, Average, and Low performance categories, with all three groups averaging approximately $6.0K.
      - Insight: This suggests that employee performance is not strongly reflected in salary levels and may indicate an opportunity for HR to review the organization's compensation structure.

 - Performance by Job Level
      - Average performance across seniority levels:
      - Entry Level: 3.05
      - Mid Level: 3.02
      - Senior Level: 2.95
      - Insight: Performance therefore did not increase with seniority in this dataset.


 - Job Level Mix by Department
      - This visual was used to examine the distribution of Entry, Mid, and Senior employees across departments.
      - Engineering showed a relatively smaller Senior-level workforce compared with their Entry-level workforce.
      - Insight: This may create a potential succession planning concern because fewer senior employees may be available to take over leadership responsibilities when experienced employees leave.
 
 - Absence by Age Group
      - Employees aged 30–39 recorded the lowest average absence at 7.45 days.
      - Employees aged 50+ recorded the highest at 7.60 days.
      - Insight: The difference is small, so age does not appear to have a strong relationship with absence in this dataset.

 - Performance by Age Group
      - Average performance remained almost the same across all age groups:
      - 20–29: 3.02
      - 30–39: 3.01
      - 40–49: 3.01
      - 50+: 2.99
      - Insight: This suggests that employee performance is not strongly dependent on age in this dataset.
 
 - Salary by Age Group
      - Average salary was approximately $6.0K across most age groups.
      - The 40–49 group had a slightly lower average salary of $5.9K.
      - Insight: Overall, there was no clear increase in salary based on age.

 - Recent Promotions by Age Group
      - Instead of using lifetime promotions, the analysis was refined to focus on promotions in 2024, the most recent complete year in the dataset.
      - The 50+ age group recorded the highest number of promotions with 294, while the 20–29 group recorded the lowest with 195.
      - Insight: This provided a more meaningful comparison than simply counting all employees with a promotion date.


### Recommendations
 
 - Review the Compensation Structure
      - HR should review whether salary increases and rewards are sufficiently connected to performance, job level, experience, and career progression.
      - Reason: The current data shows very little difference in average salary across these groups.
 
 - Review the Performance Rating Process
      - HR could review the performance review process and provide clearer guidance to managers.
      - Reason: The large number of High and Low ratings compared with Average ratings may indicate that managers are not using the full rating scale consistently.

 - Strengthen Succession Planning
      - HR could identify high-potential employees and create development plans for future leadership positions.
      - Reason: Engineering should receive special attention because of their relatively smaller Senior-level workforce.

 - Use Better Promotion Metrics
      - Future HR reports should use year-specific promotion counts or promotion rates instead of lifetime promotion counts when comparing employee groups.
      - Reason: This produces fairer and more accurate comparisons between groups of different sizes.

 - Investigate Marketing Performance
      - HR could investigate whether training, workload, management practices, or other workplace factors may be contributing to lower scores.
      - Reason: Marketing recorded the lowest average performance score.


### Assumptions

 - Performance Score
      - Values were classified using the established thresholds: Low (\le 2), Average (3), and High (\ge 4).
 
 - Job Levels
      - Grouped into Entry, Mid, and Senior categories (Levels 1, 2, and 3 respectively).
 
 - Years at Company
      - Grouped into 0\text{--}5, 6\text{--}10, 11\text{--}15, and 16\text{--}20 years.
 
 - Promotion Year
      - Derived directly from the Promotion Date.
 
 - Work Mode
      - The original Work Location field was renamed to Work Mode.
 
 - Scope
      - The analysis is descriptive and strictly reflects the information contained in the dataset. No additional assumptions were added where the project documentation did not establish them.


### Limitations
 
 - Dataset Scope
      - The analysis is based on 5,000 employee records and therefore reflects only the employees represented within this specific dataset.
 
 - Descriptive Analysis
      - The dashboard identifies patterns and relationships within the available employee data but does not establish causation (for example, differences in salary across work modes do not demonstrate that work mode causes differences in salary).
 
 - Limited Context
      - While the dataset covers performance, salary, attendance, promotions, demographics, and employment info, other broader organizational factors that may influence employee outcomes were not included.
 
 - Promotion Analysis
      - Promotion patterns are based strictly on the recorded promotion information available in the dataset.
 
 - Missing Data Documentation
      - The exact number of missing values, duplicate records, and specific missing-value treatments were not retained in the available project documentation, which should be verified directly from the final Power BI model if needed.



### Authour 
