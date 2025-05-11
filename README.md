# COVID-19 Analysis Report

- A report on the COVID-19 dataset from the PLP's week 8 assignment.

**Dataset:** [OWID - COVID-19]  
**Total entries:** 429,435 rows | 69 columns  
**Selected columns used for analysis:** ["location", "date", "total_cases", "total_deaths", "new_deaths",
"total_vaccinations", "total_tests", "new_tests", "positive_rate",
"people_vaccinated", "people_fully_vaccinated"]


## Data Cleaning

- There is a huge gap between the number of vaccinations and tests which were done verses the total number of cases recorded. There were a lot of missing values.
- Following countries were selected for the analysis:   **United States, India, Kenya, Ghana, China, Brazil, Nigeria, Australia, Sweden, Japan, Russia**

- Used forward fill(ffill) for cummulative series over time and mean for daily metries per country for the rest of the data for filling in missing values.

- Even after filling in the missing values, some rows still had missing values which were dropped. 

- Brazil and China were removed after dropping the rows with null values indicating that they had a lot of null values.


## Exploratory Data Analysis

####  **Total Cases Over Time**
- **United States** had the highest growth rate in total cases over time, followed by **India**.
- **Russia** initially showed a rise but became constant.
- **Japan** surpassed Russia in later stages.
- **Ghana, Kenya, Nigeria** had significantly fewer cases and slower growth.

####  **Total Deaths Over Time**
- Countries with highest number of cases had more deaths over time as shown.
- **United States** had a greater number of death rate over time, followed by **India** and **Russia**.
- **African countries** maintained relatively low death rates.

#### **Total Vaccinations Over Time**
- **India** had the highest vaccination rate over time.
- Followed by **United States** and **Japan**.
- Others countries showed steady but slower progress.
- African countries had a greater number of vaccinated people to the total number of cases.

#### **Total Vaccinations Over Time**
- **India** had the highest vaccination rate over time.
- Followed by **United States** and **Japan**.
- Others countries showed steady but slower progress.
- African countries had a greater number of vaccinated people to the total number of cases.



### Insights gotten
- There is a lot of missing data in terms of vaccination and testing as compared to the total cases.
- African countries had the lowest number of cases with greater rate of vaccination.
- Japan had low death rate as compared to the total number of deaths even though their cases rose over time maybe due to better containment of the virus.
- Strong correlation between total deaths and total cases.