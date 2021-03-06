# Employee Satisfaction and Performance

## Scenario

Every quarter, Pharma Drug Inc. conducts two employee surveys: an *employee satisfaction survey* and a *performance rating survey*.

Using the results from these two surveys *and* data from Pharma Drug's employee records, fashion a report on the results of the survey.  Use the ff questions as guiding principles:

* *How happy are the employees with the company?*
   - *Who is unhappy*
   - *Why are they unhappy?*
* *How happy is the company with its employees?*
   - *Who is not performing*
   - *Why are they not performing?*

## Datasets

> **Note**: the path `../../Data/*` pertains to a processed data file by jobs under the scenario's `data-source`.
>
> The path `../scenario-name/*` pertains to a processed data files under a different `scenario-name` from the same `data-source`.

| Dataset | Description | Columns | Rows | Input Data | Data Processing Scripts | csv Data File | xlsx Data File | R Data File |
|:--|:--|--:|--:|:-:|:-:|:--|:--|:--|
| Employee records | Employee database maintained by HR; collated from employee profile sheets and employee records database | 18 columns | 1,470 rows | `../../Data/data01_parsed ingest.rds` | `prep00_from parsed ingest.R` | [`Employee records.csv`](https://drive.google.com/open?id=18ad9cDTke0K17g5haW9vr8l7X9HIsV6M) | [`case_Employee Satisfaction and Performance.xlsx`](https://drive.google.com/open?id=1tpYNejB06-NvbSgA37jxpu0QAEMO8Fmg) | [`case_Employee Satisfaction and Performance.RData`](https://drive.google.com/open?id=1PnW8k9y6k6S45iaoUN2x0hFp5gP51obk) |
| Performance rating survey | Results of performance rating survey accomplished by managers | 6 columns | 1,470 rows | `../../Data/data01_parsed ingest.rds` | `prep00_from parsed ingest.R` | [`Performance rating survey.csv`](https://drive.google.com/open?id=1UJSni8l-1TKbv0LeegE8p80aQ8s9VBW6) | [`case_Employee Satisfaction and Performance.xlsx`](https://drive.google.com/open?id=1tpYNejB06-NvbSgA37jxpu0QAEMO8Fmg) | [`case_Employee Satisfaction and Performance.RData`](https://drive.google.com/open?id=1PnW8k9y6k6S45iaoUN2x0hFp5gP51obk) |
| Satisfaction survey | Results of satisfaction survey accomplished by all staff | 6 columns | 1,470 rows | `../../Data/data01_parsed ingest.rds` | `prep00_from parsed ingest.R` | [`Satisfaction survey.csv`](https://drive.google.com/open?id=1XbTDzUDbKPyz8ZTFIHRYa0u5FRxIceNl) | [`case_Employee Satisfaction and Performance.xlsx`](https://drive.google.com/open?id=1tpYNejB06-NvbSgA37jxpu0QAEMO8Fmg) | [`case_Employee Satisfaction and Performance.RData`](https://drive.google.com/open?id=1PnW8k9y6k6S45iaoUN2x0hFp5gP51obk) |

### Employee records

* __EmployeeNumber__: Employee ID
* __Sex__: *Male* or *Female*
* __Age__: Employee age
* __MaritalStatus__: *Single*, *Married*, *Divorced*
* __DistanceFromHome__: Distance of work from home (in km?).  Ranges from 1--29.  29km ~ Makati to San Pedro, Laguna
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
* __NumCompaniesWorked__: Number of companies worked with prior
* __TotalWorkingYears__: Total number of years working up to present
* __Department__<br/>
	- *Sales*
	- *Research & Development*
	- *Human Resources*
* __JobLevel__: Ranges from 1--5
* __JobRole__: Job title
* __YearsAtCompany__: Tenure
* __YearsInCurrentRole__: Years in current role
* __YearsSinceLastPromotion__: Years since last promotion
* __MonthlyIncome__: Current monthly salary
* __StockOptionLevel__: Ranges 0--3
* __SalaryHike__: Increase in salary by last promotion

### Performance rating survey

* __EmployeeNumber__: Employee ID
* __PerformanceRating__<br/>
	- *1* 'Low'
	- *2* 'Good'
	- *3* 'Excellent'
	- *4* 'Outstanding'
* __YearsWithCurrManager__: Years with current manager
* __OverTime__: *TRUE*, *FALSE*
* __TrainingTimesLastYear__: Number of trainings attended last year

### Satisfaction survey

* __EmployeeNumber__: Employee ID
* __EnvironmentSatisfaction__: *How satisfied are you with your working environment?*
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __RelationshipSatisfaction__: *How satisfied are you with the relationship with your co-workers?*
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __JobSatisfaction__: *How satsified are you with your job?*
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __JobInvolvement__: *How engaged are you at work?*
	- *1* 'Low'
	- *2* 'Medium'
	- *3* 'High'
	- *4* 'Very high'
* __WorkLifeBalance__: *How much work-life balance do you feel you have?*
	- *1* 'Bad'
	- *2* 'Good'
	- *3* 'Better'
	- *4* 'Best'