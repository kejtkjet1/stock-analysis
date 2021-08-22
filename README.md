# Stock-analysis

## Overview of Project

### Purpose

We looked at excel stock market outputs to create a program that can summarize the stock performance regardless of the year we want to analyze. We initially worked with a VBA code that performed the same function, but took a lot longer to run the code. The goal of this VBA script was to provide smilar analysis of the data but to do so for multiple years and process the data faster. 
## Results


We started the stock analysis with an original code developed while following the class module. The run time for year 2017 and 2018 was as follows

![2017_originalcode.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/2017_originalcode.png)
![2018_originalcode.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/2018_originalcode.png)

The performnance significanly improved after the code was refactored

![VBA_Challenge_2017.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/VBA_Challenge_2017.png)
![VBA_Challenge_2018.png](https://github.com/kejtkjet1/stock-analysis/blob/main/resources/VBA_Challenge_2018.png)

As the above clearly shows, the refactored code was more than 6 times faster while generating the same exact outcome. The main benefit was removal of an additional loop by including an index for one of the arrays (which summarized the stock tickers)

A simple step of creating an index:

    '1a) Create a ticker Index
    tickerindex = 0

Allowed us to refer back to the index at later stages, for example:

To increase the volume of the current tickerVolumes by using the tickerIndex variable as the index, use the following code:
tickerVolumes(tickerindex) = tickerVolumes(tickerindex) + Cells(i, 8).Value

        
        '3b) Check if the current row is the first row with the selected tickerIndex.

   
 If Cells(i - 1, 1).Value <> tickers(tickerindex) And Cells(i, 1).Value = tickers(tickerindex) Then

               tickerStartingPrices(tickerindex) = Cells(i, 6).Value
            
        End If
        
        '3c) check if the current row is the last row with the selected ticker
         'If the next row?s ticker doesn?t match, increase the tickerIndex.
        'If  Then
            
             If Cells(i + 1, 1).Value <> tickers(tickerindex) And Cells(i, 1).Value = tickers(tickerindex) Then

               tickerEndingPrices(tickerindex) = Cells(i, 6).Value
               
        '3d Increase the tickerIndex
        tickerindex = tickerindex + 1
               
               End If

Adding the index- allowed us to simplify and minimize the code and make it faster and more flexible

The excel file the incudes the entire analysis as well as VBA code can be located: https://github.com/kejtkjet1/stock-analysis/blob/main/VBA_Challenge.xlsm

## Summary

- Advantages or disadvantages of refactoring code

  - Main benefit of refactoring an existing code is having an baseline to work from so we don't need to write the code from 0
  - However a possible disadvantage from seeing a solution that works already can come from inability of finding a new way of solving a problem that may be more efficient



- Pros and cons to refactoring the original VBA script?

  - Refractored code was a lot faster- we were able to eliminate some of the loops to allow much faster processing
  - The original code on the other hand was easier to set up and comprehend - and the logic was a bit easier to follow initially
