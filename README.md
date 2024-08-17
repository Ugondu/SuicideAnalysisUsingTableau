# Uncovering Patterns and Trends in Global Suicide Data using Tableau



![image](https://github.com/user-attachments/assets/70c62d3c-6252-4d38-857b-8228d0ec1be3)


# Table of Contents

- [Objective](#objective)
- [Data Source](#data-source)
- [Design](#design)
  - [Tools](#tools)
- [Development](#development)
  - [Data Exploration](#data-exploration)
  - [Data Cleaning](#data-cleaning)
- [Visualization](#visualization)
  - [Results](#results)
  - [Calculations](#calculations)
- [Analysis](#analysis)
  - [Findings](#findings)
  - [Insights](#insights)
- [Recommendation](#recommendation)
- [Conclusion](#conclusion)



# Objective

- What is the pain point?

HealthStat are currently struglling to uncover comprehensive insights into global suicide pattern. 


- What could be the ideal solution to this business problem?

To comprehensively uncover and visualise insights into patterns, trends, and demographics in the data available, utilizing a Tableau dashboard that answers the followimg questions is key;

1. How do suicide rates vary across countries and demographic group?
2. What is the trend of suicide in age?
3. What is the trend of suicide in gender?
4. Are there correlation between economic indicators and suicide rate?
5. How has suicide rate changed over time ?

# Data Source

To answer the business problem for HealthStat, the data should include the following indices;

- Country: Name of the country where the suicide data is recorded
- Year: The year in which the suicide data is recorded
- Sex: Gender of the individuals (Male or Female)
- Suicides_No: Number of suicides reported
- Population: The total population of the specified group
- HDI For Year: Human development index for the specified year
- GDP for Year ($): Gross Democratic Product (GDP) for the specified year
- GDP per Capita ($): Gross Democratic Product (GDP) per capita for the specified year
- Generation: The generation cohort to which the individuals belong

The dataset is sourced from the company and can be found here, [see here to find it](https://github.com/Ugondu/SuicideAnalysisUsingTableau/blob/main/Assets/DataSets/Suicide%20Data.xlsx)


# Design

## Tools
| Tool | Purpose |
| --- | --- |
| Excel | Exploring, Cleaning, and analyzing the dataset |
| Tableau | Visualizing the data via interactive dashboards |
| GitHub | Hosting the project documentation |


# Development

- To create and end to end solution for our analysis, the steps will entail:

1. Get the dataset
2. Explore, clean and normalize the dataset using Excel
3. Visualize the cleaned data using Tableau
4. Generate findings based on the insights
5. Write documentation on GitHub
6. Publish and present findings

## Data Exploration

The dataset is analysed at this stage to check for errors, inconsistencies, data type error, bugs, corrupted characters, whitespaces, blanks, and null fields.

- Initial observations
1. Presence of null and blank cells
2. Contains columns not relevant to our analysis
3. Some headers were not descriptive for easy understanding

## Data Cleaning
To achieve normalisation of the dataset,

1. Irrelevant columns were removed
2. Blank and Null fields were removed


# Visualization

## Results

- Our final dashboard showing detailed insights and trends.
![image](https://github.com/user-attachments/assets/62944dde-7254-4551-925c-4d0051ca1cca)

## Calculations
- We created a calculated field to find the correlations in our analysis

### 1. Coefficient between GDP per capita and population

```tableau
WINDOW_CORR(SUM([Population]), SUM([Gdp Per Capita ($)]))
```

### 2. Coefficient between GDP per capita and Suicide

```tableau
WINDOW_CORR(SUM([Gdp Per Capita ($)]), SUM([Suicides No]))
```

### 3. Coefficient between population and Suicide

```tableau
WINDOW_CORR(SUM([Population]), SUM([Suicides No]))

```

# Analysis

## Insights
From the data made available to us, We can deduce a very high rate of suicide in the Russian Federation with over 56,000 cases reported over the period between 1985 to 2016. 
This can be associated with certain factors such as social imbalance in the Soviet region, high alcohol consumption which is prevalent in Russia, regional disparities, and the wide gap between rural and urban dewellers leading to isolation. 

Secondly, with over 77% of reported cases in this period, worldwide data suggest that men are more likely to commit suicide compared to the females. This can be correlated to the cultural norms that discourage men from expressing emotions or seeking help. Additionally, higher rates of alcohol abuse and social isolation among men. 

In the age group, we uncovered that adults over the age of 75 have attempted suicide compared to other age group in the data available. This could be due to factors like social isolation, physical health depreciation, and depression.
On the other hand, younger children between 5 and 14y have the least number with just 109 cases over period of 31 years. They are generally have good support system of parents and relatives, thus any mental health break down is tackled immediately.

In relation to economic indicators such as population and GDP per capita, there is a positive correlation between population and suicide rate which indicate increase in suicide cases with increasing population sprout. Although this may not be a direct causative factor, but it is worthwhile to consider it in further analysis. 

There is no relationship between GDP per capita and suicide rate with correlation score of 0.05 which indicates weak relationship. Although poverty has been reported as a leading cause of depression, the data available does not show that. Thus more information is required in subsequent analysis.

We further looked into how suicide rates have progressed over the years, from the data the rates peaked in 1999, 2003 and dipped considerably in 2015. This dip can be associated to the impact of awareness created over social media, economic recovery after the rcession of 2008, and improved legislations and mental health accessibility to individuals who needed help. 

From the data, we forcasted a continued dip into these numbers as rate of awareness and orientation continue to improve worldwide.

# Recommendation

1. Implementing strategies such as community based programs in regions where there is high disparities should be encouraged to prevent isolation and feeling of being alone by individuals.
2. Introduction of caregiver support to adults above 75 years will help combat the high rate of cases reported amongst this demographic.
3. Creating mental health need application or social media platforms will help improve the mental health of its users and provide support and redirection when needed 

