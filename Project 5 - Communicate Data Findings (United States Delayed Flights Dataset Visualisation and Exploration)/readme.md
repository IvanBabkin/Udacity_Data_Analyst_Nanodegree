# Project 5 - Communicate Data Findings (United States Delayed Flights Dataset Visualisation and Exploration)

This project has two parts and aims to demonstrate the importance and value of data visualization techniques in the data analysis process. The purpose of the first part is to use Python visualization libraries to systematically explore a United States Delayed Flights dataset, starting from plots of single variables and building up to plots of multiple variables. The purpose of the second part is to produce a short presentation that illustrates interesting properties, trends, and relationships that were discovered in the selected dataset. The primary method of conveying these findings will be through transforming exploratory visualizations from the first part into polished, explanatory visualizations.


## Dataset

The dataset contains data regarding flights in the United States, including carriers, flight delays, and reasons for these delays, from January 2010 to January 2021 and was manually downloaded from RITA's website in the form of a CSV file. There are 177,483 entries in the dataset. Each entry records flights of a specified airline to a specified airport during a specified month and year. Each entry provides the breakdown of causes of delayed flights in terms of the total number of flights and total delayed minutes. Excluding destination, carrier and airport names columns, which are categorical variables and are stored as strings, all other columns contain numeric values and are stored as floats.

## Main features of interest

Since the causes of delays are already clearly stated in the dataset, I am most interested in finding out what influences the total delayed minutes for every entry. My secondary objectives are: finding out how the most common delay causes are distributed and how the total delayed minutes changed in 2020 due to the pandemic.

**Note**: Only the findings for the primary investigation objective, what influences the total delayed minutes, will be mentioned in the presentation (part 2 of this project).

## Summary of Findings

**Total minutes delay findings**
* Numeric variables of total minutes delay, total arriving flights and number of delayed flights are all highly correlated with each other, where the lowest correlation between the three variables is 0.884.
* The shape, median and the quartiles of total minutes delayed between the years 2010 to 2019 seem roughly the same. However, the total minutes delay drops significantly in 2020 and 2021.
* There are no significant differences in total minutes delay between the 12 months.
* Total minutes delay have very varying distributions among the top 10 destinations. While the median seems to be roughly similar, the overall distribution is vastly different from one destination to the next.
* The distribution of total mins delay among the top 10 carriers does not follow a pattern. However, unlike the distribution for the top 10 destinations, there is a visibly significant difference in the total minutes delay median and quartiles for the top 10 carriers.

**Main causes of delay**
* The distribution of the biggest delay cause in the entries is almost identical to the distribution of the biggest minutes delay cause.
* Most common dominant cause of delays among all the entries in this dataset is the weather (58% of all entries).
* National Aviation System is the second biggest cause (34.5% of all entries).
* Late aircraft, security, and carrier causes are rarely the biggest delay causes, and each is only cited as dominant in 2-3% of all entries.

**Total delayed minutes change in 2020**
* The distribution of total minutes delay varies among the top 10 destinations. However, in 2020 the range of total minutes delay for all months is significantly higher than in 2019 for all months.
* In 2019 the total minutes delay for all top 10 destinations seems to be relatively the same throughout the 12 months. However, there are larger ranges of total minutes dealy for certain destinations during May and the summer months, but these differences are not observed for all destinations. In contrast, in 2020, the months of April, May and June have significantly smaller total minutes delay for all destinations.
* There is not much difference between 2019 and 2020 for the top 10 carriers.