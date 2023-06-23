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

1. Load the excel and CSV file into a pandas dataframe.
2. Explored missing values in the datasets by missingno library and pandas function.
3. Converting the date column to pandas’ date time format.
4. Clean the dataframe by filtering out specific countries of interest in the Primary dataset.
5. Renaming the Country ID column to “Status Count”.
6. Performed Split, Apply and Combine techniques to create appropriate result set for top10 analysis.
7. Created dataframes with status = “Closed due to COVID-19”, Partially open, Closed due to COVID- 19, Partially open. Restricted the list of countries to top 10.
8. Slice the main GDP dataframe with only "Country Name”, “Country Code", "2020"
9. Slice the UNESCO school closure dataset to keep columns 'Date’, ‘Country ID','Country','Status
10. Merge the UNESCO and GDP dataframe using 'Country ID’ and 'Country Code'.


## Analysis and Visualizations

Following analysis and data visualizations were created for understanding the school closures impact.

<div>
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/0f0d974f-52e0-49ae-85a2-7887abdee731" alt="Image 1" width="450" />
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/ad06dbc8-8607-4315-9219-f833452fbf15" alt="Image 2" width="450" />
</div>

- Bangladesh has been highly impacted with 439 days of Fully Closed school
- Panama had the longest continued fully closed schools for more than 3 quarters between March-2020 and January-2021

<div>
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/0a86c80b-d273-4e75-8fab-9b8d40baff63" alt="Image 1" width="450" />
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/69a5dcc3-f83b-401b-b96e-fd176e453cce" alt="Image 2" width="450" />
</div>


- The United States has been highly impacted with 465 days of “Partially Opened” school
- Duration wise the United States, Argentina, and Colombia had longest continued partially opened status for close to 3 quarters

<div>
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/1520f09b-9b37-4a2d-a116-0fdba3ad10df" alt="Image 1" width="450" />
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/0a8369a1-142d-44ae-86dd-fbfc5f4ba52d" alt="Image 2" width="450" />
</div>

- Solomon Islands and Singapore with 27 days of fully closed school status were in the top for the “shortest fully closed” status. 
- The majority of school closures happened between March-29 to April-12 in 2020 for this category

<div>
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/b6a69ec7-e246-4b72-838b-2111e5f45a0b" alt="Image 1" width="450" />
    <img src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/43d9f04d-d311-431b-af8a-5025c7d7b2a5" alt="Image 2" width="450" />
</div>

- Algeria and Croatia with 14 days of partially opened school status were in the top for the “shortest partially opened” status. 
- The shortest partially opened duration was observed in June 2020 and Nov 2020 for Croatia and Algeria

<img width="900" alt="image" src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/14e2e8c0-339a-4d27-8d18-69ba5aa296f9">

Belarus, Burundi, Nauru and Tajikistan did not have school closures due to Covid-19

The trend of the global school closures status for different statuses were observed with the help of time series graphs (below). The school closures became more prevalent from March to July-2020 when pandemic was on the rise. In September, a reversal in trends emerged and around 100 countries opened schools fully, while about 50 countries opened schools partially and around 25 countries kept their schools fully shut

Source: https://data.unicef.org/resources/one-year-of-covid-19-and-school-closures/

<img width="900" alt="image" src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/b06e869c-89ea-41e8-b73f-596d8c6ab422">

<img width="900" alt="image" src="https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/8f15a36b-e4ca-4b56-9f51-b0b085a8885c">

![image](https://github.com/cheerspankaj/MADS_Milestone-1/assets/82276130/8f15a36b-e4ca-4b56-9f51-b0b085a8885c)


Project Git Repository link - https://github.com/cheerspankaj/MADS_Milestone-1
