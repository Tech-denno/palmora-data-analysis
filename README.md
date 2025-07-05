# My DSA Final Project: Gender Equality and Salary Distribution Analysis at Palmora Group

## Project Summary
- Conducted a broad HR analytics case study using Power BI, focused on gender representation, salary structure, and bonus allocation in Palmora Group.
- Identified systemic gender imbalance across regions and departments, with males consistently outnumbering females on average.
- Detected a considerable gender pay gap in key departments (Services, Human Resources, and Marketing), particularly in Abuja and Kaduna.
- Provided practicable recommendations to support fairer compensation practices, enhance gender equality, and improve HR data quality.

## Project Overview:
This capstone project was completed as part of a three-month intensive Data Analytics program. It aimed to unearth insights related to gender equality and salary structure within Palmora Group using Power BI. 

### Key Objectives:
- Appraise gender representationn across regions and departments.
- Measure perceived gender equality.
- Detect potential gender pay gaps and determine areas requiring intervention.
- Analyze salary distribution by gender and region.
- Calculate bonuses and total compensation.

### Data Source:
- Palmora Group Employee Data
- Palmora Group Bonus Rules
Provided in Excel format by INCUBATOR HUB.

### Key POWER BI Concepts Used:
-  Importing and Transforming Data (ETL)
-  Creating Calculated Columns using DAX (e.g., Salary Bands):
  
   ![Calculated Column (Salary Bands)](https://github.com/user-attachments/assets/9bd29851-a617-4976-9fe9-52a74f9edd50)
   
-  Merging Tables for Unified Data Modeling:
  
   ![Merged Table](https://github.com/user-attachments/assets/61df8466-25a7-456a-b837-73950848c278)
   
-  Data Relationships and Modelling
-  Building Interactive Visualizations (bar charts, pie charts, matrix tables)

### Exploratory Data Analysis (EDA):
1. Gender Representation Across Palmora Group
1a. Overall Gender Composition

![Pie Chart](https://github.com/user-attachments/assets/671dbb85-b59e-461a-b3cd-a853332c50c2)

- The majority of employees.
- Female employees constitute a smaller proportion.
- "Undisclosed" gender entries exist, though in the minority.

1b. Gender Distribution by Region

![Clustered Column Chart](https://github.com/user-attachments/assets/518e8ec4-aaac-4d52-a9f3-6c21bf19354e)

- Abuja and Kaduna employ more people than Lagos.
- All three regions show male dominance in gender composition

1c. Gender Disribution by Department

![Stacked Column Chart](https://github.com/user-attachments/assets/3e97ba91-f0c2-4793-909e-fd8af94b40d4)

- Better gender balance in Marketing, Training, Engineering, HR, and Business Development.
- Male-dominated departments: Accounting, Sales, Support, Project Management, and Legal.
- "Undisclosed" gender values are spread across departments, emphasizing a data quality issue.

#### Key Insight:
- No department or region shows a female-majority workforce.
- Gender imbalance seems to be systemic, not isolated.
 
2. Employee Perception/Rating of Gender Equality

   ![Clustered Column Chart (2)](https://github.com/user-attachments/assets/842ff177-d45c-4b06-b5da-a4393cafe32f)

Based on internal survey ratings (e.g., Poor, Average, Good, Very Good, Very Poor):
- Majority responses fall under "Average" and "Good."
- A significant portion of these responses came from male employees.

  #### Insight:
- Employee sentiment indicates neutrality or lukewarm satisfaction regarding gender equality.
- Further awareness programs may be needed to tackle this ambiguity.
   
3. Gender Pay Gap Analysis
- Calculated the average male salary minus average female salary across departments and regions.
- Services, HR, and Marketing showed the most significant gender pay gaps.
- The gaps are most pronounced in Abuja and Kaduna.

  ![Stacked Column Chart (2)](https://github.com/user-attachments/assets/5a71d7ee-b4d5-469d-b82e-b3c619639d8b)
   
  ![Gender Pay Gap](https://github.com/user-attachments/assets/3fbfd7e5-1b76-44f1-857f-e4aabdf94981)
  
 #### Insight:
- Males are earning significantly more than females in several departments and regions.

4. Salary Band Distribution by Gender and Region
4a. Minimum Salary Benchmark Check:
- Palmora Group does not meet the $90,000 minimum salary threshold.
  - Average male salary: $75,000
  - Average female salary: $72,000

4b. Salary Band ($10,000 intervals) by Gender
- Higher salary bands (e.g., $90,000+) skew towards male.
- Females more represented in lower salary bands.
  
  ![Clustered Column Chart (3)](https://github.com/user-attachments/assets/b321dc80-bb02-477a-9711-66ec65b9c6f9)

4c. Salary Band Distribution by Region
- Abuja and Kaduna dominate higher salary brackets.
- Lagos employees are represented across all salary bands, however, their numbers are lower than those in Abuja and Kaduna.
  
  ![Clustered Column Chart (4)](https://github.com/user-attachments/assets/cd4a3610-aeb7-436b-b9db-af525003d24d) 

5. Bonus and Total Compensation Analysis
5a. Bonus Amount Calculation (Based on Matrix Table)
- Calculated for each employee using NEW MEASURE in Data View:
-  Bonus Amount = SUMX(Palmora[Salary] * Palmora[Bonus Rate])

![Matrix](https://github.com/user-attachments/assets/40cb56c4-573e-4a47-a007-f1aba433db30)

5b. Total Compensation:
- Total Compensation = SUMX(Palmora, Palmora[Salary]) + Palmora[Salary] * Palmora[Bonus Rate]))
- Combined salary and bonus for complete financial assessment.

5c. Regional Compensation Totals
- Kaduna and Abuja regions account for higher total payouts.

![Clustered Column Chart (5)](https://github.com/user-attachments/assets/553768c4-6b69-4e27-974a-916443151063)

5d. Company-Wide Total Compensation
- Aggregated sum across all employees and regions.

![Total Amount](https://github.com/user-attachments/assets/775b4f28-38ce-4942-bfac-51d176b89454)

