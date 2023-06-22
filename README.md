# Exploring effect on child's education due to school closure due to COVID-19 pandemic
## <img width="900" height="400" alt="Covid-19 School Closure" src="https://data.unicef.org/covid-19-and-children/wp-content/uploads/sites/3/2021/09/UN0500343-e1631289570701.jpg">

Image source Link:https://data.unicef.org/covid-19-and-children/


## Objectives

The objective of this GitHub repository is to explore the data available at UNICEF sites and create visualizations for the top ten countries most impacted by school closures caused by the COVID-19 pandemic. The specific goals of this project are:

Conduct time series analysis to determine the longest and shortest school closure periods during the pandemic.
Calculate the total number of children-days-closed, representing the cumulative impact of school closures on education.
Investigate the correlation between school closures and the relative GDP of the affected countries.
By analyzing and visualizing this data, the project aims to shed light on the extensive disruptions to education caused by the pandemic and raise awareness about the long-term consequences of these disruptions.

## Datasets

Primary dataset: The primary dataset details the status of school closures by region and country.

Link: https://covid19.uis.unesco.org/global-monitoring-school-closures-covid19/

Secondary dataset : The datasets have information about the country's GDP over time.

Link: https://data.worldbank.org/indicator/NY.GDP.MKTP.CN

## Data Manipulation Methods


Generic steps.

1.Load the excel and CSV file into a pandas dataframe
2.Explored missing values in the datasets by missingno library (Figure 1) and pandas function
3.Converting the date column to pandas’ date time format
4.Clean the dataframe by filtering out specific countries of interest in the Primary dataset.
5.Renaming the Country ID column to “Status Count”
6.Performed Split, Apply and Combine techniques to create appropriate result set for top10 analysis.
7.Created dataframes with status = “Closed due to COVID-19”, Partially open, Closed due to COVID- 19, Partially open. Restricted the list of countries to top 10.
8.Slice the main GDP dataframe with only "Country Name”, “Country Code", "2020"
9.Slice the UNESCO school closure dataset to keep columns 'Date’, ‘Country ID','Country','Status
10.Merge the UNESCO and GDP dataframe how='inner’, left_on='Country ID’, right_on='Country Code'


## Analysis and Visualizations

Following analysis and data visualizations were created for understanding the school closures impact.
### longest and shortest school closures period from February 2020 to October 2021 using time series analysis
<img src="![image](https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/dd1daca1-8dc1-40dd-a0f8-16c62e0960c5)
" alt="Title" width="500" height="300">




Project Git Repository link - https://github.com/cheerspankaj/MADS_Milestone-1
