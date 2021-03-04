# Regression Analysis of Snapchat Political Ads
## Background
Snapchat records data on political ads for every year. This information includes when the campaign took place, how much was spent, who the advertisement was for, and lots of info about what demographics to target the ad towards. I decided to analyze the current year, this made it easier because I could use current exchange rates, and the larger data sets of past years crashed my excel twice so I decided the smaller set was best. 
## Business Question
Can you predict the number of impressions for a political advertisement on snapchat?

## Analysis
I performed a multiple variable  linear regression to try and see how money spent and the length of the campaign. Let X1 be the amount spent in USD, X2 be the length of the campaign in hours, and Y be the number of Impressions.

Y = 311.567X1 + 0.927X2 - 59170.5

This was the equation generated from the regression. It had an R Square of 0.9646 and a F significance of 0. These are very good but analyzing the p values revealed that the length of the campaign had a value of 0.966, while the others were less than .001. This means that only money spent really affects impressions, and not the length of the campaign.
So I did a simple linear regression with just money spent and imprssions. This resulted in the graph below, where X is amount spent and Y is impressions.

![alt text](https://github.com/cmclane1/Regression_Analysis_of_Snapchat_Political_Ads/blob/main/Impressions_vs_Money_Spent.png)
As the equation and R squared shows, money spent alone is a very good predictor of impressions, which makes a lot of sense since snapchat would want companies to be incentivized to pay as much as possible for ad viewing. 

## Step by Step Walkthrough
I wanted to analyze the length of the campaign and the amount spent. I converted the time interval into hours by reconstructing the date and using the datedif excel function. Because I was using ongoing data there were current campaigns and I used if statements check for this. Then I just used the current date. These time intervals were left in hours. I then used nested if statements to convert the spent amount to USD using the current exchange rate I found on google. I then used regression tools on the data, more in the analysis section. 
  
## Links to Sources
[Analysis](https://github.com/cmclane1/comparing-baltimore-bristol-county-household-income/blob/main/Baltimor-Bristol-Analysis.xlsx)

[Data](https://github.com/cmclane1/comparing-baltimore-bristol-county-household-income/blob/main/Baltimore-Bristol-Data.xlsx)
