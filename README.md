# HealthStat Suicide Analysis Using Tableau.
*![image](https://github.com/Ugondu/SuicideAnalysisUsingTableau/assets/113315492/6e1f9931-852c-4110-8042-9ca5327502c9)*
## Table of Contents.
- [Business Problem Overview](#business-problem-overview)
- [Project Objective](#project-objective)
- [Data Sources](#data-sources)
- [Data Processing](#data-processing)
- [Insights and Findings](#insights-and-findings)
- [Conclusion and Recommendation](#conclusion-and-recommendation)
## Business Problem Overview.
HealthStat Analytics is a global health analytics company committed to understanding and addressing mental health challenges. The company is currently facing difficulties in analyzing global suicide data to identify patterns, risk factors, and demographic trends. Therefore, there is a need to explore and visualise the available dataset to extract meaningful insights for effective mental health interventions.
## Project Objective. 
The aim of the project is to use Tableau to perform a thorough exploratory data analysis on the available dataset, uncovering patterns, correlations, and trends to inform evidence-based public health strategies and interventions.
To achieve the business objectives.
1.	Examine how suicide rates vary across countries and demographic groups.
2.	Evaluate if there are notable trends in suicide rates based on age and gender.
3.	Establish the correlation between economic indicators such as GDP and suicide rates.
4.	Explore how suicide rate has changed over time in different countries.
5.	Identify countries and regions with high or low suicide rates.

## Data Sources.
The datasets were made available by 10alytics data consulting team.
### data dictionary:
* Country: Name of the country where the suicide data is recorded.
* Year: The year in which the suicide data is recorded.
* Sex: Gender of the individuals (Male or Female).
* Suicides_No: Number of suicides reported.
* Population: The total population of the specified group.
* Country-Year: Concatenation of country and year, serving as a unique identifier for each record.
* HDI For Year: Human development index for the specified year.
* GDP for Year ($): Gross Democratic Product (GDP) for the specified year.
* GDP per Capita ($): Gross Democratic Product (GDP) per capita for the specified year.
* Generation: The generation cohort to which the individuals belong.
## Data Cleaning.
* Missing Values: The blank fields were removed from the dataset.
* Duplicates: Duplicates values were removed from the dataset.
* Removal of non-relevant columns: “HDI” was removed from the dataset as it contained many missing cells.
## Insights and Findings.
* Our analysis shows that out of 6,748,420 reported cases, 77% were males, while 23% are females. Over the period of years available in the data, 1999 was the year with most suicide case, with the Russian Federation having the most cases of all the countries reported.
* Based on GDP per capita, suicide rates peaked in the year 2008 with 235,447 cases, from year 1985 until 1994, there was steady and constant increase of suicide case per capita. In the year 2016, the number tanked to 15,000 reported cases.
* In relation to population, there were reported cases of 243,000 in 2009, with a steep decrease in the year 2015.
* There is a positive correlation between population and suicide rate while GDP had no impact on the number of reported cases in the data available.
* Given the number of reported cases over the years, our forecast shows that suicide cases will continue to reduce between 2016 and 2018.
## Conclusion and Recommendations
This showcases the effectiveness of visualisation tools such as Tableau in providing useful insights in available data over a period of time. We are able to show the forecast how many suicide cases will be reported in 3 years after the data was made available. 

