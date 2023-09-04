# Power-BI-CarAccidentAnalysis

Road Accident Dashboard
Road Accident Dashboard for 2021 and 2022 This project aims to create a road accident dashboard using Power BI for the years 2021 and 2022. The dashboard will provide insights into various aspects of road accidents based on the provided requirements. The primary Key Performance Indicators (KPIs) include Total Casualties and Total Accidents, Total Casualties by Accident Severity for the current year, and Total Casualties with respect to Vehicle Type. The dashboard will also include Monthly Trend analysis, Casualties by Road Type, Casualties by Area/Location and Day/Night, and Total Casualties and Total Accidents by Location.
Functionalities in Power BI The following functionalities in Power BI will be utilized to create the dashboard:

**Loading of CSV file**: The road accident data for 2021 and 2022 will be loaded from a CSV file into Power BI for analysis.

**Data cleaning using Power BI:** Power BI provides various data transformation and cleaning tools to handle missing values, remove duplicates, and format data for analysis.

**Time intelligence function:** Power BI offers built-in time intelligence functions to perform calculations and comparisons based on date/time fields. This will be useful for analyzing the Monthly Trend and other time-based analyses.

**Creating KPIs:** Key Performance Indicators (KPIs) will be defined in Power BI to track and visualize the primary metrics, such as Total Casualties and Total Accidents, and Total Casualties by Accident Severity for the current year.

**Grouping:** Power BI allows grouping of data based on specific attributes, such as Vehicle Type, Road Type, and Location, which will help in analyzing Casualties with respect to Vehicle Type, Casualties by Road Type, and Total Casualties and Total Accidents by Location.

**Creating a dashboard:** Power BI provides a user-friendly interface to create interactive and visually appealing dashboards. Visualizations such as charts, graphs, and maps will be used to present the analysis results.


**STEP IN PROJECT**

	Requirement Gathering

	Data Overview

	Connecting Data with Power bi

	Data Cleaning

	Data Modeling

	Background Design in Power Point

	Data Visualization and Charts Designs

	Dashboard Building

	Insights

**REQUIREMENT**

Clients want to create a Road Accident Dashboard for Year 2021 and 2022 so that they can have insight on the below requirements:-

	Primary KPI – Total Casualties and Total Accident values for Current Year and YOY growth.

	Primary KPI - Total Casualties By Accident Severity for Current Year and YOY growth.

	Secondary KPI – Total Casualties with respect to vehicle type for Current year

	Monthly Trend showing compression of casualties for current year and previous year.

	Casualties By Road type for current year.

	Current year casualties by Area wise

	Current year casualties by Location wise

	Current year casualties by Day/Night wise

	Total Accident and Total casualties by Location 


**POWER BI FUNCTIONALITES**

	How to connect a raw data in power bi
  
	Data Cleaning in power query
  
	Data Processing
  
	Create a calendar table by using time intelligence function
  
	Data Modeling (Relationship b/w Multiple tables)
  
	YTD and YoY Growth calculation by using DAX Expressions
  
	KPI and Advance KPI generation

	Creating Custom Column 
  
	Creating a Calculated measures 
  
	Import images
  
	Creating a different Charts for visualization

**Data Cleaning in power query: -**

-	Found Spell mistake under Accident severity (Like Fetal and Fatal) – corrected.
  
-	Checked quality of all the columns – no issues found.
  
**Data Processing: -**

-	Create a calendar/Date table by using time intelligence function – Calendar/CalendarAuto function
  
    DimDate = CALENDAR(FIRSTDATE(Data[Accident Date]),LASTDATE(Data[Accident Date]))
    DimDate = CALENDAR(MIN(Data[Accident Date]),MAX(Data[Accident Date]))

-	Created new calculated columns like – YEAR, MONTH, WEEKDAY, FORMAT, CONCATENATE, QUARTER, WEEKEND....
Data Modeling (Relationship b/w Multiple tables):

-	We have created relaltionship between DIMDATE and Data Table.(ONE -TO- MANY)
KPI and Advance KPI generation: -

-	YTD and YoY Growth calculation by using DAX Expressions
  
-	Creating a Calculated measure
  
-	causality
  
**	Find out current year causality by using TotalYTD function.**

**	Find out pervious year causality by using below function.**

    •	 Calculate + SAMEPERIODLASTYEAR
    •	 Calculate + DateADD

**	Find out YOY causalities by using**

    •	Divide((CY – PY)/PY)*100

-	Accident
**	Find out current year Accident by using TotalYTD function.**
 	
**	Find out pervious year Accident by using below function.**

    •	Calculate + SAMEPERIODLASTYEAR
    •	Calculate + DateADD

**	Find out YOY Accident by using**

    •	Divide((CY – PY)/PY)*100

**	Find out current year casualties by accident severity – Fatal, Serious, Slight**

**	Created new group and covert type of vehicle into single entity.**

**Import images**

-	We have use some vehicle pics for better visualization.
Creating a different Charts for visualization

-	We have used below chart to show trends
  
**	Area chart to show trend related to CY vs PY Casualties.**

**	Multi-row card to show KPI values related to vehicle type**

**	Bar chart to show casualties by Road type.**

**	Pie chart to show Accident happened by light condition and severity**

**	Card to show KPI values.**

**	Map visual to show causalities by location using longitude and latitude(Avg)**

 
 

