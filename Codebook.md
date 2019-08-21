
# Stranger things on Electricity Consumption: Codebook
*Íngrid Munné Collado*

*Data Analytics June 2019*

In this document all the information regarding all the datasets used for this project are described, including the features, their description and the units of measurement. 

## **information_households.csv**

Information about each household and their tariff. 

| Feature name   | Description  | Units     |
| :------------- | :---------- | -----------: |
|  LCLid         | Household ID | [-]           |
| Tariff   |Type of tariff contract | [Std or ToU]  |
| Acorn   |Associated acorn group  | [-]  |
| Acorn_grouped   |  acorn group details  | [-]  |
| file   |file name or hourly block on this user appears  | [-]  |



## **acorn_details.csv**
20 columns containing information about how to classify end-users according to 68 indicators 

| Feature name   | Description  | Units     |
| :------------- | :----------: | -----------: |
|  MAIN CATEGORIES         | Social Indicators where acorn group is split into | [Population, Economy, Education, Health, Transport,...]           |
|  CATEGORIES         | Indicators where acorn is measured | [Age, Country of Birth, Religion, House Type,... ]           |
| Reference          | Units on which that indicator is measured | [years, type of religion,  Occupation ]  |
| ACORN-A            | Values for that indicator on that ACORN group | [based on Reference]  |
| ACORN-B            | Values for that indicator on that ACORN group | [based on Reference]  |
| ACORN-B            | Values for that indicator on that ACORN group | [based on Reference]  |
| ACORN-C            | Values for that indicator on that ACORN group | [based on Reference]  |
| ACORN-D            | Values for that indicator on that ACORN group | [based on Reference]  |
| ACORN-E            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-F            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-G            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-H            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-I            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-J            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-K            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-L            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-M            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-N            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-O            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-P            | Values for that indicator on that ACORN group | [based on Reference] |
| ACORN-Q            | Values for that indicator on that ACORN group | [based on Reference] |## 



## **weather_hourly_darksky.csv**

 csv file containing information on the weather in a hourly scale. It contains 12 columns: 

| Feature name   |  Units     |
| :------------- | -----------: |
|visibility | [-]
|windBearing | [-]
|Temperature |  [ºC]
|Date Time | [datetime object]
|dewPoint | [ºC]
|pressure | [mbar]
|apparentTemperature |  [ºC]
|windSpeed |  [m/s]
|precipType | [-]
|icon | [-]
|humidity | [%]
|summary | [-]



## **halfhourly_dataset.zip or folder**

This folder contain 112 blocks. Each block is a .csv file containing data of the different households at a half hourly scale.

In this case, each row contains one user and one halfhour period. There are three columns:

| Feature name   | Description  | Units     |
| :------------- | :---------- | -----------: |
|  LCLid         | Household ID | [-]           |
| Timestamp   |Day and hour of the measurement  | [YYYY-MM-DD HH:MM:SS]  |
| Consumption   |Energy consumption in that time period  | [kWh]  |



## **hhblock_dataset.zip or folder**

This folder contains 112 blocks. It contains the same information as halfhourly_dataset in terms of data. In this case, each row is one user for day; and each column is one half-hour for that day, with the energy consumption on that day. 



## **daily_STATS_datasets_blocks.zip or folder**

Folder containing 112 blocks. Each block contains information about the energy consumption of that end-user in that day: 

| Feature name   | Description  | Units     |
| :------------- | :---------- | -----------: |
|  LCLid         | Household ID | [-]           |
| Day   |Day of the measurement  | [YYYY-MM-DD]  |
| Energy_median   |Energy consumption median in that day | [kWh]  |
| Energy_mean   |Energy consumption mean in that day | [kWh]  |
| Energy_max   |Energy consumption maximum in that day | [kWh]  |
| Energy_count   |Energy consumption count in that day | [-]  |
| Energy_std   |Energy consumption Standard Deviation in that day | [kWh]  |
| Energy_sum   | Total energy consumption in that day | [kWh]  |
| Energy_min   |Energy consumption min in that day | [kWh]  |

## **daily_STATS_datasets_one_file.gz Zip file**

Zip folder containing the same information as above but in only one file. 

