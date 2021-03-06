# [IBM Watson HR Employee Attrition](https://www.ibm.com/communities/analytics/watson-analytics-blog/guide-to-sample-datasets/)

> Find out the leading drivers of Employee Attrition. Track and analyze employee satisfaction and retain valuable employees.

## Data Files

### [Raw data files](https://drive.google.com/open?id=1Aezowz0EZbknJAJqykC4PG6VIj11KodG)

| Filename | Description | Source | Documentation | Columns | Rows | Size |
|:---------|:------------|:-------|:--------------|--------:|-----:|-----:|
| `WA_Fn-UseC_-HR-Employee-Attrition.csv` | Collated employee records and survey results | [Watson Analytics](https://community.watsonanalytics.com/wp-content/uploads/2015/03/WA_Fn-UseC_-HR-Employee-Attrition.csv) | [Kaggle](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset) | 35 columns | 1,470 rows | 227,977 bytes |

### [Parsed data files](https://drive.google.com/open?id=1DH7K1KfKAMBOkpaGd5pEn8wtcQ5ZDfqu)

| Data file | Description | Columns | Rows | Input data | Processing script |
|:--|:--|--:|--:|:--|:--|
| `data00_raw ingest.rds` | Loaded raw data | 35 columns | 1,470 rows | `WA_Fn-UseC_-HR-Employee-Attrition.csv` | `script00_raw ingest.R` |
| `data01_parsed ingest.rds` | Cleaned raw data | 29 columns | 1,470 rows | `data00_raw ingest.rds` | `script01_inspect and parse.ipynb` |

## Datasets

### `WA_Fn-UseC_-HR-Employee-Attrition.csv`

#### Schema

* __Age__
* __Attrition__: Has employee left the company: *Yes*, *No*
* __BusinessTravel__<br/>
	- *Travel_Frequently*
	- *Travel_Rarely*
	- *Non-travel*
* __DailyRate__<br/>
* __Department__<br/>
	- *Sales*
	- *Research & Development*
	- *Human Resources*
* __DistanceFromHome__<br/>
* __Education__<br/>
	- *1* 'Below College'
	- *2* 'College'
	- *3* 'Bachelor'
	- *4* 'Master'
	- *5* 'Doctor'
* __EducationField__<br/>
	- *Human Resources*
	- *Life Sciences*
	- *Marketing*
	- *Medical*
	- *Technical degree*
	- *Other*
* __EmployeeCount__: Dummy column
* __EmployeeNumber__: Employee ID
* __EnvironmentSatisfaction__<br/>
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __Gender__: *Male*, *Female*
* __HourlyRate__<br/>
* __JobInvolvement__<br/>
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __JobLevel__: Ranges from 1--5
* __JobRole__: Job title
* __JobSatisfaction__<br/>
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __MaritalStatus__: *Single*, *Married*, *Divorced*
* __MonthlyIncome__
* __MonthlyRate__
* __NumCompaniesWorked__
* __Over18__: All *Yes*
* __OverTime__: *Yes*, *No*
* __PercentSalaryHike__<br/>
* __PerformanceRating__<br/>
	- *1* 'Low'
	- *2* 'Good'
	- *3* 'Excellent'
	- *4* 'Outstanding'
* __RelationshipSatisfaction__<br/>
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __StandardHours__: All *80*
* __StockOptionLevel__: Ranges 0--3
* __TotalWorkingYears__
* __TrainingTimesLastYear__
* __WorkLifeBalance__<br/>
	- *1* 'Bad'
	- *2* 'Good'
	- *3* 'Better'
	- *4* 'Best'
* __YearsAtCompany__
* __YearsInCurrentRole__
* __YearsSinceLastPromotion__
* __YearsWithCurrManager__

### Sample

| Age | Attrition | BusinessTravel | DailyRate | Department | DistanceFromHome | Education | EducationField | EmployeeCount | EmployeeNumber | EnvironmentSatisfaction | Gender | HourlyRate | JobInvolvement | JobLevel | JobRole | JobSatisfaction | MaritalStatus | MonthlyIncome | MonthlyRate | NumCompaniesWorked | Over18 | OverTime | PercentSalaryHike | PerformanceRating | RelationshipSatisfaction | StandardHours | StockOptionLevel | TotalWorkingYears | TrainingTimesLastYear | WorkLifeBalance | YearsAtCompany | YearsInCurrentRole | YearsSinceLastPromotion | YearsWithCurrManager |
|--:|:-:|:-:|--:|:--|--:|:-:|:--|--:|:-:|:-:|:-:|--:|:-:|:-:|:--|:-:|:-:|--:|--:|--:|:-:|:-:|--:|:-:|:-:|--:|:-:|--:|--:|:-:|--:|--:|--:|--:|
| 41 | Yes | Travel_Rarely | 1102 | Sales | 1 | 2 | Life Sciences | 1 | 1 | 2 | Female | 94 | 3 | 2 | Sales Executive | 4 | Single | 5993 | 19479 | 8 | Y | Yes | 11 | 3 | 1 | 80 | 0 | 8 | 0 | 1 | 6 | 4 | 0 | 5 |