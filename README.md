# Factors Impacting the Use of Telehealth for Medicare and Medicaid Members in 2020-2024

* This Research Data Analytics project focuses on factors that are associated with an increase of decrease in number of telehealth For Medicare and Medicaid Populations.

## Motivation

* This research can be used to understand potential socioeconomic barriers to telehealth access to aid opportunities for targeted interventions to improve equitable access to care.

## Authors & Collaborators 

* Jessie Coomber completed this project. 
* Dr. Alexandre Scarcioffolo supported its progress.

## Data and Results Folder

### Preliminary Results RMD and Preliminary Results HTML

* This HTML and Rmd were used for initial results. This document is updated into the Results Draft documents.

### Results Draft RMD and Results Draft HTML

* This HTML file includes the data cleaning, data exploration, prediction forecasting, and interpretations.

* The Rmd file that was used to create the HTML file is also included. An individual will need to have an R studio installed to run this file.

### Data 

#### 1. Medicare Telehealth Trends.csv
* Data from the U.S. Department of Health & Human Services which is publicly available through Data.gov. Used to assess telehelath utilization for Medicare and Medicaid members.
* Variable definitions were found in the Medicare Telehealth Trends Data Dictionary file

#### 2. Tenure by Vehicles Available_2020.csv (_2021.csv, _2022.csv, _2023.csv, _2024.csv)
* Publicly available data from the US Census Bureau to assess vehicle access. Merged with Medicare Telehealth Trends.csv based on state.

#### 3. Presence and Types of Internet Subscriptions_2020.csv (_2021.csv, _2022.csv, _2023.csv, _2024.csv)
* Publicly available data from the US Census Bureau to assess internate access. Merged with Medicare Telehealth Trends.csv based on state.

#### 4. CentersForMedicareAndMedicaidServicesFacilities Hospitals.csv
* Data from the Health Resources and Services Administration (HRSA) to assess the number of hospitals and providers. Merged with Medicare Telehealth Trends.csv based on state.

#### 5. Annual Estimates of the Resident Population for the United States.csv
* Publicly available data from the US Census Bureau to merge population size by state.
* This variable is used to convert other variables into per capita format.

#### 6. Transit Report Card.csv
* Transportation for America to capture individuals public transportation spending. Merged with Medicare Telehealth Trends.csv based on state.

#### 7. UNRATE.csv and GDP.csv
* Federal Reserve Economic Data (FRED) annual GDP in billions and unemployment rate as a percentage. Merged to the Medicare Telehealth Trends dataset based on year

### Methodology
* 7 variables have been chosen for the multivariable fixed effect model in relation to telehealth visits. 
* The variables include: the number of vehicles owned, transit spending per capita, having internet access, number of hospitals, number of physicians, GDP, and unemployment rate.
* Variance Inflation Factor (VIF) analysis is used to test for multicollinearity which could lead to unreliable coefficient estimates and impact the interpretation.


