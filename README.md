# Dutch Electricity and Gas

## Introduction
Analysis from the seven biggest energy providers in the Netherlands about electricity and gas consumption from the years 2013 to 2018 was conducted. The analysis was aimed at uncovering and understanding trends related to energy consumption, regional and provider differences and the key factors that affect them. Insights and recommendations geared towards making informed decisions about promotion of new energy efficient programs, smart meter adoption and infrastructure relating to renewable energy.
Table of Contents

## Objectives
Energy Consumption Analysis: To assess patterns related to energy consumption and key factors that affect them
Smartmeter Analysis:  To investigate trends relate smart meter adoption
Self-Production Analysis: To analyse city and country wide trends that relate renewable energy and self reliance

## Data Description
The analyst is based on a rich dataset encompassing several key aspects to the Dutch energy system.

Geographical Details: Geographical data that details the regions where the providers operate at a regional, zip, city and street level. This information can be used to

Connection Details: The information provides details for connections in terms of where they are located, if they’re active, how many there are, and the type of connection. This can be used to 

Consumption Details: The datasets provide information related to the amount energy consumed overall, how much was given back to the grid and when they were consumed.

The use of geographical, connection and consumption details allow for a deeper understanding about the production of Dutch energy, and in turn the action required to increase sustainable energy use. By focusing on key factors and their effects, effective steps can be undertaken. 

The SQL queries used to inspect and clean the data for this analysis can be found here

DAX measures used in power query can be found here

## Data Structure and Checks
Excel Power Pivot was used to combine 8 million records from 150 files from kaggle and separate them into 2 different datasets, one for electricity and one for gas. A description for both unedited and edited data structure is as follows:

## Executive Summary

For electricity, the oligopoly of Stedin, Liander and Enexis made up 97% of energy consumption in the country and 91% of gas consumption. Stedin is based in the regions of Rotterdam, Arnhem and Amsterdam. Liander throughout the idle of the country and Enexis in both south and northern outskirts. All other companies have niche markets that they supply to, E.g Endurise in the South-west on the France border.

Since 2014 there has been a noticeably downward trend in delivery percentage for all companies due to the rise of renewable energy. The lowest of which being Enexis at 84%.and the highest being Stedin at 91%. Westland Infra has the highest smart meter adoption at 37% (electricity) and 34% (gas), while Endinet has the lowest at 5% (electricity)  and 4% (gas). For gas there has been a slight decline in gas consumption for all companies bar a few outlier years.

To further push for sustainable living it is crucial to understand the behaviours and patterns the population undertakes when consuming energy. This report provides an in-depth analysis about energy consumption, smartmeter use and overall self production. By examining these findings, we can identify both successes and areas for further improvement.

## Insights Deep Dive
### Energy Consumption

Total electricity consumption seems to be roughly consistent over the past 8 years, however there has been a slight decline with Liander and Stedin. In the same time frame the number of connections has grown linearly since 2012. This means that the consumption per connection has decreased, possibly due to large scale adoption of more energy-efficient products such as LED-lights. Looking deeper at cities consumption per connection, the 20 biggest cities are in the rural areas in the northeast of the country. This can be attributed to those cities being placed in windy rural parts of the country, allowing for easy access and use of wind turbines and solar panels.

Gas consumption has been on a steady decline from a peak of 1908 m3 in 2013 to a low of 1724m3 in 2019. However, the count of gas connections during the same time grew from 6.7 million to a peak of 7.3 million in the same time period. This further means that in terms of consumption per connection that Dutch households are consuming less gas. Decrease in gas consumption likely stems from the growth in renewable energy and overall energy efficiency improvement because of the additions of solar power, heat pumps and already in place government incentives. Unlike with electricity, the highest consumption per household is not limited to one part of the country as it is spread out across the major cities.

### Smartmeter
Electrical smartmeter adoption has been growing exponentially up until 2020. The electricity sector is at 72% adoption and at this rate it is expected that the complete transition might take around 30 more years. Additionally, smartmeter percentage is positively correlated with the rise of low tarif consumption, this effect is most predominantly seen in Liander cities. However, it is likely other factors are also affecting the increase in low tariff consumption in the country.

For gas connections, smartmeter adoption has increased tenfold since 2013, from an average of 5% to 54% in 2019, at this rate it is expected that full smart meter adoption will be completed within the next 7 years. There is no rise in low tariff consumption likely due to the different price structures between electricity and gas. Electricity grids use time-of-use pricing, where lower tariffs apply at night or during low-demand periods. Gas pricing, however, is usually fixed or seasonal, not hourly.

### Self Production
Overall, looking at providers individually there is a trend of self-production growing in all regions since around 2012, with Enexis outperforming the other regions.The north-east region where Enexis operates has more space for windmills and solar panels to be placed. On the other hand, Stedin cities are the slowest at increasing self production, due to having their cities inside the populated central region of the country. Enexis cities have the space they need to set up renewable energy systems as they sit on the outskirts of the country. It is easier for smaller towns in these regions to obtain a high percentage of self-produced electricity than the larger cities, again due to the space available. Furthermore, urbanisation may have a limit towards the amount of renewable energy they can produce themselves as these areas come with their own types of problems. For example, flats in high-rise buildings do not have the option to place solar panels.

## Conclusion
Continue to push smartmeter use especially in the Coteq and Endinet regions
Expand renewable energy in rural areas to potential handle more cities such as the ones in Stedin
High smart meter adoption suggests openness to smarter energy use and potential market to push programs. Focus on connections such as 1x25 for electricity and g6 for gas.

## Recommendations
While all stats for delivery % is down Stedin has the slowest decline of all providers. High smart meter adoption suggests openness to smarter energy use and potential market to push programs. Furthermore, very low smart meter adoption for Coteq and Endinet providers suggest push for adopting should be focused in these markets. 
Lastly, customers with 1x25 connections also show low adoption.

## Technical issues with the dataset:
The province of Zeeland seems to be missing entirely, but this could be due to there being a fourth provider
Something is wrong with the historical (pre-2017) data for Eindhoven
Some cities seem to have multiple providers. This might actually be true, but seems unlikely for some larger cities in Enexis territory like Weert and Deventer
Some cities seem to be producing gas, this seems unlikely
There are many minor errors, such as 's Gravenhage appearing more than once (but overall I ignore this since there is one 's Gravenhage that is the right size, the others are almost negligibly small.
