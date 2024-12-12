---
output:
  html_document: default
  pdf_document: default
---


# Electricity Generation and Environmental Justice Communities in North Carolina

## UshasriPriceHeschong_ENV872_EDE_FinalProject

This project aims to analyze electricity generation in North Carolina, with a specific interest in solar generation and impact on Environmental Justice communities.

## Summary
The researchers' interest in Energy and Environmental Justice motivated the topic of this project. Specifically, the goal is to understand how power generation impacts Environmental Justice communities. Since solar power is a robust renewable energy source in North Carolina, solar power plants will also be a focus in this investigation.

This analysis plans to address the following research questions:

1. What is the distribution and capacity of power plants generating electricity in North Carolina?
2. Does electricity generation impact air quality through criteria air pollutant emissions in North Carolina?
3. What are the Environmental Justice implications of electricity power generation in North Carolina? Are power plants primarily located in low-income and disadvantaged communities?


## Investigators
Asreeta Ushasri, Summer Heschong, Fiona Price

## Keywords
Solar Power, North Carolina, Environmental Justice Communities, Electricity Generation

## Database Information
EGRID 2022: The U.S. Environmental Protection Agency publishes data on the status of electricity generation, the location of power plants, and generator fuel types each year. This data set describes electricity generation in the United States as of 2022. https://www.epa.gov/egrid/download-data Accessed in November 2024.

CEJST 2022: The U.S. Council on Environmental Quality publishes data to map climate and economic justice in the United States. This database includes findings from the climate justice screening tool for 2022. https://screeningtool.geoplatform.gov/en/methodology#3/33.47/-97.5 Accessed in November 2024.

Details for the processed data can be found in the Data Wrangling and Processed RMD.

## Folder structure, file formats, and naming conventions
This repository contains a folder with the relevant data, including Raw, Processed and Spatial. The Data Wrangling and Processing RMD file depicts how the raw data sets were compiled for the analysis.

## Metadata

### Raw Data

Table: CEJST Data

|Item | Value|
|:-------------|:-------------|
|Filename | CEJST_data.csv|
|Date | 2022|
|Source | U.S. Climate and Economic Justice Screening Tool|
|Link | https://screeningtool.geoplatform.gov/en/methodology|
|Column Names | Please see the CEJST_ColumnNames file in the Metadata folder within the Data folder. The CEJST-communities-list and CEQ-CEJST-Instructions documents describe the data collection methodology as well.|

Table: EGRID Data

|Item | Value|
|:-------------|:-------------|
|Filename | egrid2022_data.xlsx|
|Date | 2022|
|Source | U.S. Environmental Protection Agency|
|Link | https://www.epa.gov/egrid/download-data|
|Column Names | Please see the EGRID2022ColumnNames_Contents file in the Metadata folder within the Data folder. The EGRID2022_Technical_Guide describes the data collection methodology as well.|

### Processed Data

Table: NC Energy Emissions

|Item | Value|
|:-------------|:-------------|
|Filename | NC_Energy_Emissions.csv|
|Source | U.S. Environmental Protection Agency|
|Link | https://www.epa.gov/egrid/download-data|
|Column Names and Descriptions | |
|"Plant primary fuel category" | This is the main source of fuel used by the power plant to generate electricity|
|"total_CO2e" | This is the CO2 equivalent emissions in tons.|

Table: NC Environmental Justice CSV

|Item | Value|
|:-------------|:-------------|
|Filename | NC_Env_Justice.csv|
|Source |  U.S. Climate and Economic Justice Screening Tool|
|Link | https://screeningtool.geoplatform.gov/en/methodology|
|Column Names and Descriptions | Please see the CEJST_ColumnNames file in the Metadata folder within the Data folder.|

Table: NC Environmental Justice GPKG

|Item | Value|
|:-------------|:-------------|
|Filename | NC_Env_Justice.gpkg|
|Source |  U.S. Climate and Economic Justice Screening Tool|
|Link | https://screeningtool.geoplatform.gov/en/methodology|
|Column Names and Descriptions | Please see the CEJST_ColumnNames file in the Metadata folder within the Data folder.|

Table: NC Power Plants and Environmental Justice CSV

|Item | Value |
|:-------------|:-------------|
|Filename | NC_joined.csv |
|Source |  U.S. EPA and U.S. Climate and Economic Justice Screening Tool |
|Link | https://www.epa.gov/egrid/download-data and https://screeningtool.geoplatform.gov/en/methodology |
|   | |
|Column Descriptions | |
|     | |
|County Name | |
|Data Year | |           
|Plant state abbreviation | |
|Plant name | |                        
|Utility name | |
|Plant latitude | |
|Plant longitude | |
|Number of units | |
|Number of generators | |
|Plant primary fuel category  | |
|Plant nameplate capacity (MW) | |
|Plant annual net generation (MWh) | |
|Plant annual NOx emissions (tons)  | |
|Plant annual SO2 emissions (tons)   | |
|Plant annual CO2 emissions (tons) | |
|Plant annual CH4 emissions (lbs) | |
|Plant annual N2O emissions (lbs) | |
|Plant annual CO2 equivalent emissions (tons) | |
|Percentage of Community which Identifies as Black | |
|Percentage of Community which Identifies that race is not applicable | |
|Percentage of Community which Identifies as Asian | |                   
|Percentage of Community which Identifies as Hawaiian | |
|Percentage of Community which Identifies with Two Communities | |
|Percentage of Community which Identifies as White | |
|Percentage of Community which Identifies as Hispanic | |
|Counties Classified as Disadvantage | |
|Population | |
|Percent of Community Facing Poverty | |
|Levels of PM 2.5 in Air Quality | |


Table: NC Power Plants and Environmental Justice GPKG

| Item | Value |
|:-------------|:-------------|
|Filename | nc_plants_EJ.gpkg|
|Source |  U.S. EPA and U.S. Climate and Economic Justice Screening Tool|
|Link | https://www.epa.gov/egrid/download-data and https://screeningtool.geoplatform.gov/en/methodology|
|Column Descriptions | Binary file, utilized for shape/geometry in maps|

Table: NC Power Plants

|Item | Value |
|:-------------|:-------------|
|Filename | NC_PowerPlants.csv|
|Source |  U.S. EPA|
|Link | https://www.epa.gov/egrid/download-data|
|   | |
|Column Descriptions | |
|     | |
|Data Year | |           
|Plant state abbreviation | |
|Plant name | |                        
|Utility name | |
|County Name | |
|Plant latitude | |
|Plant longitude | |
|Number of units | |
|Number of generators | |
|Plant primary fuel category  | |
|Plant nameplate capacity (MW) | |
|Plant annual net generation (MWh) | |
|Plant annual NOx emissions (tons)  | |
|Plant annual SO2 emissions (tons)   | |
|Plant annual CO2 emissions (tons) | |
|Plant annual CH4 emissions (lbs) | |
|Plant annual N2O emissions (lbs) | |
|Plant annual CO2 equivalent emissions (tons) | |


Table: NC Electricity Generation Capacity

|Item | Value|
|:-------------|:-------------|
|Filename | NC_Total_Capacity.csv|
|Source | U.S. Environmental Protection Agency|
|Link | https://www.epa.gov/egrid/download-data|
|Column Names and Descriptions | |
|"Plant primary fuel category" | This is the main source of fuel used by the power plant to generate electricity |
|"total_capacity" | This is the sum of the nameplate capacity of all the power plants under that fuel category in North Carolina in MW.|

## Scripts and code
The repository includes a Data Wrangling and Processing RMD file, which contains the code to write the processed data sets. The Data Wrangling file showcases which worksheets in the EGRID 2022 data set were utilized in this analysis. The repository also contains a Data Exploration RMD file, which examines the column names of the processed data sets and includes the code for initial exploratory analysis.

The individual analyses folder contains three RMD files which were initial explorations by members on the research team, and one blank example of the final project template. Each researcher analyzed one of the three research questions in an individual RMD file, before compiling into the final product.