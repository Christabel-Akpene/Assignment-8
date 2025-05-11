# COVID-19 Analysis Report (PLP Week 8)

- A data analysis project using the OWID COVID-19 dataset to examine global trends in cases, deaths, testing, and vaccination rollouts. The analysis focuses on selected countries to understand the pandemic's progression and response across different regions.


##  Objectives

- To understand the progression of COVID-19 cases and deaths across various countries.
- To analyze vaccination rollouts and their relationship to cases recorded.
- To visualize trends using line charts, bar charts and heatmaps.
- To derive insights from the data.


##  Tools & Libraries Used

- **Python** 
- **Pandas** – for data manipulation and cleaning
- **Matplotlib** – for visualizations
- **Seaborn** – for plots and heatmaps

## ⚙️ How to Run the Project

1. Read the dataset.
2. Run the Jupyter Notebook (`covid_analysis.ipynb`) in your preferred Python environment.
3. Install required libraries using:
   ```bash
   pip install pandas matplotlib seaborn plotly


## Data Cleaning

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