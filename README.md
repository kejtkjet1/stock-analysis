# Stock-analysis

## Overview of Project

### Purpose

We looked at excel stock market outputs to create a program that can summarize the stock performance regardless of the year we want to analize. We initially worked with a VBA code that performed the same function, but took a lot longer to run the code. The goal of this VBA script was to provide smilar analysis of the data but to do so for multiple years and process the data faster. 
## Results


We started the stock analysis with an original code developed while following the class module. The run time for year 2017 and 2018 was as follows

![2017_originalcode.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/2017_originalcode.png)
![2018_originalcode.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/2018_originalcode.png)

The performnance significanly improved after the code was refactored

![VBA_Challenge_2017.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/VBA_Challenge_2017.png)
![VBA_Challenge_2018.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/VBA_Challenge_2018.png)

One of the main challenges encountered with this data set was UNIX Timestamp used to signify the deadline and the launch date. We were able to overcome this challenge by converting the UNIX Timestamp to a usable date format by applying a formula that converted seconds since January 1, 1970 to an actual date. This allowed us to understand the timeframes for each fundraiser. 

## Summary

- Advantages or disadvantages of refactoring code

  - One important piece of infomration is the fundraising campaign lenghth. It would help to evaluate if longer or shorter fundraising campaigns generated more successful outcomes  
  - We should re-create the visualizations above for outcomes that look at the target market only. While its helpul to evaluate Kickstarter campaigs for all the markets, we will not get a clear picture unless we only look at the country we are intersted in. Each market may be affected by regional nuances
  - We should also recreate the vizualizations above looking at more recent years only. While looking at a larger data set allows us to see seasonality, the marketplace surely has changed significantly since 2009. A look at more recent years may provide more relevant information to base our decision on
  - We shold also create a visualization that looks at percentage success based on average donation by backer. It will help us evaluate if more successful plays depended heavily on couple of large donations, or if the success depended on numberous smaller donors showing a mass appeaf of the play. 



- Pros and cons to refactoring the original VBA script?

  - One important piece of infomration is the fundraising campaign lenghth. It would help to evaluate if longer or shorter fundraising campaigns generated more successful outcomes  
  - We should re-create the visualizations above for outcomes that look at the target market only. While its helpul to evaluate Kickstarter campaigs for all the markets, we will not get a clear picture unless we only look at the country we are intersted in. Each market may be affected by regional nuances
  - We should also recreate the vizualizations above looking at more recent years only. While looking at a larger data set allows us to see seasonality, the marketplace surely has changed significantly since 2009. A look at more recent years may provide more relevant information to base our decision on
  - We shold also create a visualization that looks at percentage success based on average donation by backer. It will help us evaluate if more successful plays depended heavily on couple of large donations, or if the success depended on numberous smaller donors showing a mass appeaf of the play. 


