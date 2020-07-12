# S&P 500 recovery from the COVID-19 crash
This foreceast was submitted by Silviu Sica and Robert Bozsik as Project 2 during the Data Analytics Bootcamp of Ironhack Berlin.

# Task:
The goal of this project was to practice creating and interpreting different types of visualizations using real world data as well as statistical analysis.

# Project details:
We tried to predict the days of recovery of the S&P 500 index. Therefore we analyzed the historical crises.

We defined a crisis as:
 - the adjusted close price decreased more than 20% compared to the all time high
 - the price returned back to the all time high.
 
After identifying 11 historical crisis, we calculated the absolute percentage loss and the das of recovery of each. \
Then we created a polynomial regression model in order to predict the recovery of the current fall of S&P 500. \
On the 19th of February 2020 the adjusted closing price was 3386.15, that we take as all time high. \
On the 23rd of March 2020 the adjusted closing price was 2237.49, which we consider as the lowest point. \
Percentage loss is equal to -33.9%.

Based on our model (Adj. R-squared: 0.957) the recovery of the S&P 500 from the corona crash will take:
 - in days: 905.65 days,
 - in months: 30.19 months,
 - in years: 2.48 years.

The recession started on 2020-02-19 and will last until 2022-08-12.

# Resurces:
Raw data: https://finance.yahoo.com/ \
Analysis idea:
- https://www.ig.com/uk/news-and-trade-ideas/coronavirus-impact-on-the-stock-market
- http://www.mooncap.com/wp-content/uploads/2018/03/MCM.bear-markets.Mar2016.pdf 

# Tech Stack:
Python: https://www.python.org/ \
Pandas: https://pandas.pydata.org/ \
NumPy: https://numpy.org/doc/stable/reference/generated/numpy.arange.html \
Matplotlib: https://matplotlib.org/ \
Seaborn: http://seaborn.pydata.org/ \
statsmodels API: https://www.statsmodels.org/stable/index.html \
Jupyter Notebook: https://jupyter.org/ \
Tableau: https://www.tableau.com/
