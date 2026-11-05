# HR Analytics Dashboard: Employee Attrition Analysis (Power BI)

An interactive Power BI dashboard that analyses why employees leave. It breaks attrition down by age group, salary slab, job role, education field, gender, tenure and department, so HR can focus retention efforts where they matter most.

![Dashboard]<img width="1008" height="568" alt="image" src="https://github.com/user-attachments/assets/05e428c5-87d8-4101-ad69-26bdb8ba7ff5" />

**Live Dashboard:** <add your Power BI Service / published link here>

## Business Problem
Employee turnover is expensive. HR leaders need to know **who is leaving, where, and why**, so they can reduce attrition with targeted actions instead of blanket policies.

## Dataset
- File: `HR_Analytics.csv`, 1,480 rows x 38 columns (1,470 unique employees; 10 rows are repeated Employee IDs)
- Target: `Attrition` (Yes / No)
- Key fields: Age, AgeGroup, Department, JobRole, JobLevel, MonthlyIncome, SalarySlab, OverTime, BusinessTravel, MaritalStatus, JobSatisfaction, WorkLifeBalance, YearsAtCompany, EducationField, Gender

## Tools & Technologies
Power BI Desktop, DAX, Power Query

## Dashboard Contents
- **KPI cards:** Employee count, Attrition count, Attrition rate, Average age, Average monthly salary
- **Charts:** Attrition by education field, age group, salary slab, job role, years at company, gender; job role vs job satisfaction matrix
- **Slicer:** Department filter

## Key Insights
Figures below are calculated on unique employees (1,470).

- **Overall attrition is about 16%** (237 of 1,470 employees).
- **Overtime is the strongest driver.** Employees working overtime leave at about 31%, compared with about 10% for those who don't.
- **Young employees leave the most.** The 18-25 group has about 36% attrition, versus about 9% for ages 36-45.
- **Low pay means higher attrition.** The "Up to 5k" salary slab shows about 22% attrition; the 15k+ slab only about 4%.
- **Sales Representatives are the highest-risk role** (about 40%), followed by Laboratory Technicians (about 24%) and HR (about 23%). Research Directors are the lowest (about 2.5%).
- **Sales has the highest department attrition** (about 21%) compared with R&D (about 14%).
- **Single employees leave twice as often** as married ones (about 25% vs 12%).
- **Leavers earn less and have shorter tenure.** Average monthly income is about $4.8K for leavers vs $6.8K for stayers, and average tenure is 5.1 vs 7.4 years.

## Recommendations
1. Review overtime policies and workload, especially in Sales and Lab roles.
2. Strengthen early-career retention: mentoring, career paths and pay reviews for employees under 26.
3. Revisit compensation for the lowest salary slab and for Sales Representatives.
4. Run stay interviews with employees who have low job satisfaction or low work-life balance.

## Data Notes
- 10 Employee IDs appear twice in the source file (7 rows are exact duplicates). Removing them gives 1,470 unique employees.
- `BusinessTravel` contains an inconsistent label (`TravelRarely` vs `Travel_Rarely`) that should be standardised in Power Query.
- `YearsWithCurrManager` has 57 missing values.
- Attrition rate shows correlation, not causation.

## Repository Contents
```
├── HR Analytics Dashboard.pbix   # Power BI report
├── HR_Analytics.csv              # source data
├── BG12.jpg                      # dashboard background
└── screenshots/                  # dashboard images
```

## How to Use
1. Download `HR Analytics Dashboard.pbix` and open it in Power BI Desktop.
2. If prompted, point the data source to `HR_Analytics.csv`.
3. Use the Department slicer and the charts to explore attrition patterns.

## Author
Murali Krishna | [LinkedIn](#) | [Email](#)
