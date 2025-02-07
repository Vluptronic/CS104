# Homework 1 - Data munging and Linear Regression
Brandeis University
COSI 104-A Intro to Machine Learning
Spring 2025
Authors: Dylan Cashman and Binyamin Friedman


## Task
Please submit the [Jupyter notebook file](submissionPA1EricHJan25.ipynb) with your implementations. 

## Data Dictionary
This is for [training_data.csv](training_data.csv). Note that [sample_data.csv](sample_data.csv) is a different dataset.

| **Column Name**         | **Description**                                                                              | **Source**                |
|-------------------------|----------------------------------------------------------------------------------------------|---------------------------|
| TARGET_deathRate        | Dependent variable. Mean per capita (100,000) cancer mortalities                             | (a) 2010-2016             |
| avgAnnCount             | Mean number of reported cases of cancer diagnosed annually                                   | (a) 2010-2016             |
| avgDeathsPerYear        | Mean number of reported mortalities due to cancer                                            | (a) 2010-2016             |
| incidenceRate           | Mean per capita (100,000) cancer diagnoses                                                   | (a) 2010-2016             |
| medianIncome            | Median income per county                                                                     | (b) 2013 Census Estimates |
| popEst2015              | Population of county                                                                         | (b) 2013 Census Estimates |
| povertyPercent          | Percent of populace in poverty                                                               | (b) 2013 Census Estimates |
| studyPerCap             | Per capita number of cancer-related clinical trials per county                               | (a) 2010-2016             |
| binnedInc               | Median income per capita binned by decile                                                    | (b) 2013 Census Estimates |
| MedianAge               | Median age of county residents                                                               | (b) 2013 Census Estimates |
| MedianAgeMale           | Median age of male county residents                                                          | (b) 2013 Census Estimates |
| MedianAgeFemale         | Median age of female county residents                                                        | (b) 2013 Census Estimates |
| Geography               | County name                                                                                  | (b) 2013 Census Estimates |
| AvgHouseholdSize        | Mean household size of county                                                                | (b) 2013 Census Estimates |
| PercentMarried          | Percent of county residents who are married                                                  | (b) 2013 Census Estimates |
| PctNoHS18_24            | Percent of county residents ages 18-24 highest education attained: less than high school     | (b) 2013 Census Estimates |
| PctHS18_24              | Percent of county residents ages 18-24 highest education attained: high school diploma       | (b) 2013 Census Estimates |
| PctSomeCol18_24         | Percent of county residents ages 18-24 highest education attained: some college              | (b) 2013 Census Estimates |
| PctBachDeg18_24         | Percent of county residents ages 18-24 highest education attained: bachelor's degree         | (b) 2013 Census Estimates |
| PctHS25_Over            | Percent of county residents ages 25 and over highest education attained: high school diploma | (b) 2013 Census Estimates |
| PctBachDeg25_Over       | Percent of county residents ages 25 and over highest education attained: bachelor's degree   | (b) 2013 Census Estimates |
| PctEmployed16_Over      | Percent of county residents ages 16 and over employed                                        | (b) 2013 Census Estimates |
| PctUnemployed16_Over    | Percent of county residents ages 16 and over unemployed                                      | (b) 2013 Census Estimates |
| PctPrivateCoverage      | Percent of county residents with private health coverage                                     | (b) 2013 Census Estimates |
| PctPrivateCoverageAlone | Percent of county residents with private health coverage alone (no public assistance)        | (b) 2013 Census Estimates |
| PctEmpPrivCoverage      | Percent of county residents with employee-provided private health coverage                   | (b) 2013 Census Estimates |
| PctPublicCoverage       | Percent of county residents with government-provided health coverage                         | (b) 2013 Census Estimates |
| PctPubliceCoverageAlone | Percent of county residents with government-provided health coverage alone                   | (b) 2013 Census Estimates |
| PctWhite                | Percent of county residents who identify as White                                            | (b) 2013 Census Estimates |
| PctBlack                | Percent of county residents who identify as Black                                            | (b) 2013 Census Estimates |
| PctAsian                | Percent of county residents who identify as Asian                                            | (b) 2013 Census Estimates |
| PctOtherRace            | Percent of county residents who identify in a category which is not White, Black, or Asian   | (b) 2013 Census Estimates |
| PctMarriedHouseholds    | Percent of married households                                                                | (b) 2013 Census Estimates |
| BirthRate               | Number of live births relative to number of women in county                                  | (b) 2013 Census Estimates |
