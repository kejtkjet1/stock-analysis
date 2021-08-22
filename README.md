# Kickstarting with Excel

## Overview of Project

### Purpose

We analyzed data from Kickstarter dataset to help Louise set fundraising goals for her play Fever. We analyzed how different fundraising campaigns fared in relation to their launch dates as well as funding goals 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

We looked at all the theater category fundraisers and compared the outcomes based on the fundraiser launch month. The below visualization shows how many fundraisers were successful, how many failed and how many were cancelled based on the campaign launch month since 2009

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/87611145/129303868-3249bac4-c8d4-4fed-b9ab-e951200348c6.png)

### Analysis of Outcomes Based on Goals

We looked at all the plays to evaluate what fundraising budget goals generated most successful campaigns. The visualization below depicts percentage successful, failed and cancelled plays based on the goal.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/87611145/129303893-7264ca58-dd6e-41e1-bcdb-073ae7a26544.png)

### Challenges and Difficulties Encountered

One of the main challenges encountered with this data set was UNIX Timestamp used to signify the deadline and the launch date. We were able to overcome this challenge by converting the UNIX Timestamp to a usable date format by applying a formula that converted seconds since January 1, 1970 to an actual date. This allowed us to understand the timeframes for each fundraiser. 

## Results

- Conclusions from evaluating outcomes based on launch dates
  - Most of the campaigns launched in May and it appears that campaigns launched that month had the highest chance of success
  - December had the lowest number of successful campaign launches. Nearly half of the campaigns launched that month failed

- Conclusions from evaluating outcomes based on goal
  - The lower budget campaigns had much higher success percentage. The most successful campaigns had goals of up to 5K.  There is an uptick of successful campaigns between 35K-45K goal, but nearly all Kickstarter campaigns above that goal failed.

- Dataset Limitations

  - The data only looks at fundig from Kickstarter, there are additional ways to collect fundraising for plays or theater productions. Additionaly we only see the fundraising goals, not the actual budgets for each play. 
  - While we are seeing fundraising goals, not all of them are listed in USD. In order to truly understand the budget goals we would need to apply an exchange rate to convert all the currencies to one uniform currency. Alternatively, we would should evaluate the data only on a market by market basis. 
  - The dataset only includes campaigns till 2017. The world has changed significantly since that year, and so did the economy in those markets. We need to keep in mind that we are making conclusions while looking at historical, and not very recent data. 

- Additional tables and graphs we could create to dive deeper

  - One important piece of infomration is the fundraising campaign lenghth. It would help to evaluate if longer or shorter fundraising campaigns generated more successful outcomes  
  - We should re-create the visualizations above for outcomes that look at the target market only. While its helpul to evaluate Kickstarter campaigs for all the markets, we will not get a clear picture unless we only look at the country we are intersted in. Each market may be affected by regional nuances
  - We should also recreate the vizualizations above looking at more recent years only. While looking at a larger data set allows us to see seasonality, the marketplace surely has changed significantly since 2009. A look at more recent years may provide more relevant information to base our decision on
  - We shold also create a visualization that looks at percentage success based on average donation by backer. It will help us evaluate if more successful plays depended heavily on couple of large donations, or if the success depended on numberous smaller donors showing a mass appeaf of the play. 



