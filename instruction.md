## 1 Deriverable

- HTML knit markdown file and PDF report

## 2 Task Context:

In this dataset project, we are interested in analyzing the relationship between population growth and CO2 emissions. We have data for world population and CO2 emissions. The population dataset contains different features such as county names, population density, population growth rate, population ranking, world population percentage, and so on.

## 3 Task Objectives

- Implementation of data management skills.

- Exploratory data analysis

- Prepare a dataset for analysis

- Use visualization tools for population trend

- Correlation analysis

- Creating new variable from existing ones.

## 4 Task description

## 4.1 Downloading data and load them to R studio

- Visit Kaggle and download population dataset clicking here, and download two csv files entitled World Population Dataset [URL 🔗](https://www.kaggle.com/datasets/iamsouravbanerjee/world-population-dataset)

- On kaggle download CO2 Emissions Around the World here [URL 🔗]( https://www.kaggle.com/datasets/koustavghosh149/co2-emission-around-the-world)

- Load both World Population Dataset and CO2 Emissions Around the World to your R studio


## 4.2 Exploratory data analysis

In this section, you are required to use World Population Dataset display variable names, the top 5 rows, the bottom 10 rows, the data type, and the shape of the dataset. Drop duplicate rows if any, find the number of missing values in each column, and use a box plot to check if there are any outliers in the quantitative variables. Use appropriate methods to deal with missing values and outliers, if any.

## 4.3 Generating new Variable by usingWorld Population Dataset

Given that A simple equation for population projection can be expressed as:

```math
N_t = Pe^{rt}
```

In this equation:Nt is the number of people at a future date, P:Present popula- tion, e :natural logarithm base(2.71828), r: growth rate, t :time period. Use word population data-set and the formula given to predict population for each country in 2030, given that P is a number of people at the end of 2022.

## 4.4 Value extraction and plot

Based on 2022 population, extract top ten countries with high population number and use ggplot2 to perform the following task:

- 1. Use an appropriate graph to present top 10 most populous counties and their population number during 2022.

- 2. Show the trend in their population number since 1990-2022 by using appro- priate graph.

- 3. Use CO2 Emissions Around the World dataset to extract emission of 10 most populous countries. Use an appropriate graph to show their emission trend since 1990-2019.

## 4.5 Correlation Analysis

- 1. Use the population dataset to find correlations between Area , Density , Growth rate, and World Population Percentage by using both numerical values and heatmap.

- 2. Merge the World Population Dataset and CO2 Emissions Around the World on country name . After extracting, 2022 population and 2019 CO2 emis- sions.Using an appropriate methods(visualization, statistical analysis of nu- merical values,regression,...), determine the pattern of relationships between population number and CO2 emissions.


## 4.6 Comparing CO2 Emissions in continents

Use the merged datased 2. Sum 2019 CO2 emissions by continents. Use a graph- ical method to compare the CO2 emission of the continents. Based on the graph generated, answer the following: [URL 🔗](#page-0)

- 1. What is the first continent with high 2019 CO2 emission?

- 2. What is the third continent in terms of emitting CO2? What is their total emission(metric tons per capita)?

- 3. What is the last continent in terms of emitting CO2? What their total emis- sion(metric tons per capita)?

## 4.7 Report

By using latex, provide a short(max 3 pages) report that contains, an abstract (maximum 250 words), introduction, Methods used (including a description of the dataset), results findings(consider Parts 4.2, 4.3, 4.4, 4.5, and 4.6), Discussions, Lessons learned and recommendations, and a conclusion.

