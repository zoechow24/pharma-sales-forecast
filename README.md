# Pharmaceutical Sales Forecasting

## Overview
This project simulates a real-world scenario where a pharmaceutical company needs to prepare fiscal year-end sales forecasts and presentation materials for senior leadership. The goal was to analyze provided data, generate insights, and create visual assets to support executive-level decision-making.

## Scenario

### Background
The end of the fiscal has arrived and Dr. Alicia Kerns, the CFO for Plaxium LLC, needs to get ready for a presentation to the senior leadership team at the next offsite. Last week, Alicia was attending a presentation and the presenter showed, what she thoughts, was a nice and effective chart. She felt that it was a well done visualization as it was simple and got the point across. For her upcoming presentation she wants to include a similar chart in her presentation deck, so she calls you to assist her. She took a photo of the chart with her phone and sent it to you. 

![Sales Forecast Chart](https://northeastern.instructure.com/courses/206741/files/32748675/preview)

Your task is to take the data that was prepared by Arjun Patel in the CFO's Office and create a similar graph -- matching what is shown below as closely as possible (but keeping in mind that the sample graph was not done using R). In addition, she would like to add a forecast for the next two months on the chart as well. Alicia knows she'll also need a few other charts and perhaps some tables for her slide deck. 

### Tables
Alicia needs to show how revenue and expenses vary from quarter to quarter, so she beliees several tables would prove helpful. Create tables for each of the following use cases:
1. Quarterly revenue per year
2. Revenue, expenses, and profit-loss per month averaged across the years
3. Percentage change in revenue, expoenses, and profit-loss from the prior month for each year

### Forecast
Knowing that she will be asked for a forecast for revenue and expense, Alicia is asking you to make a simple forecast using a weighted moving average(WMA) of the prior three months with weights of 0.6, 0.3, and 0.1 where 0.6 is the weight for the most recent month.

### Visualization
The visualization that Alicia needs for her presentation should match what is shown in the picture she sent as closely as possible. Naturally, you need to adjust the title to "Profit & Loss By Month" and the subtitle "Trend Over Time". You should set the source for the data to "Internal Accounting Data -- CONFIDENTIAL". Adjust the axis labels as appropriate given the new data. The values are in US$ and are in thousands, e.g., a value of 23.6 means US$23,600. The blue line should show "profit/loss", i.e., the difference between revenue and expenses. The red line should be the three month weighted moving average for the prior three months, so for March 2024 it should be the WMA of March, February, and January. Use weights of (0.6,0.3,0.1) where 0.6 is the weight for the most recent month.

## Tools
* RStudio

## Methodology
1. Load data from [URL](https://s3.us-east-2.amazonaws.com/artificium.us/datasets/pharma-sales-randomized.tsv)
2. Prepare and shape data
     a. Format data
     b. Handle outliers and missing data
     c. Handle dates
     d. Calculate profit and losses
3. Aggregate data in tables
4. Make a forecast
5. Build visualization
   

