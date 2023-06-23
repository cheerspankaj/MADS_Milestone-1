# Exploring effect on child's education due to school closure due to COVID-19 pandemic
## <img width="900" height="400" alt="Covid-19 School Closure" src="https://data.unicef.org/covid-19-and-children/wp-content/uploads/sites/3/2021/09/UN0500343-e1631289570701.jpg">

Image source Link:https://data.unicef.org/covid-19-and-children/


## Objectives

The objective of this project is to explore the data available at UNICEF sites and create visualizations for the top ten countries most impacted by school closures caused by the COVID-19 pandemic. The specific goals of this project are:

* Conduct time series analysis to determine the longest and shortest school closure periods during the pandemic.
* Calculate the total number of children-days-closed, representing the cumulative impact of school closures on education.
* Investigate the correlation between school closures and the relative GDP of the affected countries.

By analyzing and visualizing this data, the project aims to shed light on the extensive disruptions to education caused by the pandemic and raise awareness about the long-term consequences of these disruptions.

## Datasets

Primary dataset: The primary dataset details the status of school closures by region and country.

Link: https://covid19.uis.unesco.org/global-monitoring-school-closures-covid19/

Secondary dataset : The datasets have information about the country's GDP over time.

Link: https://data.worldbank.org/indicator/NY.GDP.MKTP.CN

## Data Manipulation Methods


The data manipulation steps include:

1.Load the excel and CSV file into a pandas dataframe.
2.Explored missing values in the datasets by missingno library and pandas function.
3.Converting the date column to pandas’ date time format.
4.Clean the dataframe by filtering out specific countries of interest in the Primary dataset.
5.Renaming the Country ID column to “Status Count”.
6.Performed Split, Apply and Combine techniques to create appropriate result set for top10 analysis.
7.Created dataframes with status = “Closed due to COVID-19”, Partially open, Closed due to COVID- 19, Partially open. Restricted the list of countries to top 10.
8.Slice the main GDP dataframe with only "Country Name”, “Country Code", "2020"
9.Slice the UNESCO school closure dataset to keep columns 'Date’, ‘Country ID','Country','Status
10.Merge the UNESCO and GDP dataframe using 'Country ID’ and 'Country Code'.


## Analysis and Visualizations

Following analysis and data visualizations were created for understanding the school closures impact.

## Countries with Longest Fully Closed schools between Feb-2020 and Oct-2021

## <img width="900" height="400" alt="Image-1" src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/40ad02ba-1bdf-4ccf-956e-105a8cf4429c">

![image](https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/40ad02ba-1bdf-4ccf-956e-105a8cf4429c)


Bangladesh has been highly impacted with 439 days of Fully Closed school.

## Top 10 Countries with Longest School Closure between Feb-2020 and Oct-2021

![image](https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/7684112f-70c9-42d7-861e-b12a1565fa75)


Panama had the longest continued fully closed schools for more than 3 quarters between March-2020 and January-2021.





Project Git Repository link - https://github.com/cheerspankaj/MADS_Milestone-1
