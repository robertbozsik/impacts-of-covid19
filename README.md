# S&P 500 recovery from the COVID-19 crash
This foreceast was submitted by Silviu Sica and Robert Bozsik as Project 2 during the Data Analytics Bootcamp of Ironhack Berlin.

# Task:
The goal of this project was to practice creating and interpreting different types of visualizations using real world data as well as statistical analysis.

# Data sourcing and data cleaning:
The project data was sourced from yahoo finance as csv and was imported as pandas dataframe object. Additional columns were added to the dataframe (E.g: abs_percentage_loss, days_of_recovery). For the analysis we considered to focus on the adjusted close price of the index, to account for the changes in stock prices from corporate actions (E.g: dividends, stock splits).

# Project details:
Given the coronavirus crisis which caused a market crash, we tried to predict the days of recovery of the S&P 500 index. Therefore we analyzed historical market crises, with a significant impact on the S&P 500 index, taken as a market proxy.

We defined a crisis as:
 - the adjusted close price decreased more than 20% compared to the all time high
 - the price returned to the highest pre-crash value.
 
After identifying 11 historical crisis (including The Great Depression, The dot-com crash, and The Great Recession), we calculated the absolute percentage loss and the days of recovery (time-to recovery) of each event. \
Then we created a polynomial regression model in order to predict the recovery of the current fall of S&P 500. \
On the 19th of February 2020 the adjusted closing price was 3386.15, which was considered as the highest pre-crash value. \
On the 23rd of March 2020 the adjusted closing price was 2237.49, considered as the lowest drop point. \
Percentage loss (independent variable) was equal to -33.9%.

Based on our model (Adj. R-squared: 0.957) the recovery of the S&P 500 from the corona crash will take:
 - in days: 905.65 days,
 - in months: 30.19 months,
 - in years: 2.48 years.

The recession started on 2020-02-19 and will last until 2022-08-12.

The detailed analysis can be found in the [recessions_without_new_lows.ipynb](recessions_without_new_lows.ipynb) notebook.

# Project presentation:
https://docs.google.com/presentation/d/1AYtcn2SHYqswh0gmduJhVwyiMd9RpgvsxewJVwPHiD0/edit?usp=sharing

# Resources:
Raw data: 
 - https://finance.yahoo.com/
 - https://fred.stlouisfed.org/
 
Analysis idea:
 - https://www.ig.com/uk/news-and-trade-ideas/coronavirus-impact-on-the-stock-market
 - http://www.mooncap.com/wp-content/uploads/2018/03/MCM.bear-markets.Mar2016.pdf 

# Tech stack:
Python: https://www.python.org/ \
Pandas: https://pandas.pydata.org/ \
NumPy: https://numpy.org/ \
Matplotlib: https://matplotlib.org/ \
Seaborn: http://seaborn.pydata.org/ \
statsmodels API: https://www.statsmodels.org/stable/index.html \
Jupyter Notebook: https://jupyter.org/ \
Tableau: https://www.tableau.com/
