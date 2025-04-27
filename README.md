# Factors Impacting the Use of Telehealth for Medicare and Medicaid Members in 2020-2024

* This Research Data Analytics project focuses on factors that are associated with an increase of decrease in number of telehealth For Medicare and Medicaid Populations.

## Motivation

* This research can be used to understand potential socioeconomic barriers to telehealth access to aid opportunities for targeted interventions to improve equitable access to care.

## Authors & Collaborators 

* Jessie Coomber completed this project. 
* Dr. Alexandre Scarcioffolo supported its progress.

## Data and Results Folder

### Files - Final Results RMD and Final Results HTML

* * This HTML file includes the data cleaning, data exploration, prediction forecasting, and interpretations.

* * The Rmd file that was used to create the HTML file is also included. An individual will need to have an R studio installed to run this file.

### Dataset Folders found within the "Data and Results Folder"

### Telehealth Dataset
#### 1. Medicare Telehealth Trends.csv
* Data from the U.S. Department of Health & Human Services which is publicly available through Data.gov.
* Used to assess telehealth utilization for Medicare and Medicaid members.
* Variable definitions were found in the Medicare Telehealth Trends Data Dictionary file, also included in this folder.

### Vehicles Datasets
#### 2. Tenure by Vehicles Available_2020.csv (_2021.csv, _2022.csv, _2023.csv, _2024.csv)
* Publicly available data from the US Census Bureau to assess vehicle access.
* Owning vehicles is the variable that is used to represent economic status.
* Merged with Medicare Telehealth Trends.csv based on state and year.

### Internet Datasets
#### 3. Presence and Types of Internet Subscriptions_2020.csv (_2021.csv, _2022.csv, _2023.csv, _2024.csv)
* Publicly available data from the US Census Bureau to assess internet access.
* Internet Access Variable is also used to represent socioeconomic status.
* Merged with Medicare Telehealth Trends.csv based on state and year.
* 
### Poverty Datasets
#### 4. Poverty Status in the past 12 months_2020.csv (_2021.csv, _2022.csv, _2023.csv, _2024.csv)
* Publicly available data from the US Census Bureau on percent below poverty level.
* The percentage below the poverty level definied by the US Census is the variable that is used to represent poverty level.
* Merged with Medicare Telehealth Trends.csv based on state and year.

### Hospital Dataset
#### 5. CentersForMedicareAndMedicaidServicesFacilities Hospitals.csv
* Data from the Health Resources and Services Administration (HRSA) to assess the number of hospitals and providers.
* The number of hospitals is important in relation to accessible resources.
* Merged with Medicare Telehealth Trends.csv based on state.

### Tranportation Dataset
#### 6. Transit Report Card.csv
* Transportation for America to capture individuals public transportation spending.
* Higher transport spending is typical in urban areas. Urban and rural areas face many differences which could impact telehealth use.
* Merged with Medicare Telehealth Trends.csv based on state.

### Population Dataset
#### 8. Annual Estimates of the Resident Population for the United States.csv
* Publicly available data from the US Census Bureau to merge population size by state.
* This variable is used to convert other variables into per capita format.

### Merged Dataset
#### 9. TelehealthandPopulation_VehicleInternetHospitalPoverty_GDPUNRATE_Transit.xlsx
* This is the excel file exported from R, of the merged data from all the csv files listed above.
* This is the dataset used for the fixed effect analysis.

### Methodology
* 6 variables have been chosen for the multivariable fixed effect model in relation to telehealth visits. 
* The variables include: the number of vehicles owned, transit spending per capita, having internet access, number of hospitals, number of physicians, and poverty Level,.
* Variance Inflation Factor (VIF) analysis is used to test for multicollinearity which could lead to unreliable coefficient estimates and impact the interpretation.

### Output
* There are bar graph visualizations to explore the telehealth dataset including telehealth visits by rural/urban status, by race, and by year.
* The Fixed Effect model is used to display the assocation of selected factors on teh number of telehealth visits, while controling for state and year fixed effects.
* The VIF table checks for multicolinearity, confirming the interpretability of the fixed effect model.
