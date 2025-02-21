# Dutch Electricity and Gas

## Introduction
Analysis from the seven biggest energy providers in the Netherlands about electricity and gas consumption from the years 2013 to 2018 was conducted. The analysis was aimed at uncovering and understanding trends related to energy consumption, regional and provider differences and the key factors that affect them. Insights and recommendations geared towards making informed decisions about promotion of new energy efficient programs, smart meter adoption and infrastructure relating to renewable energy.

# Table of Contents

- [Objectives](#Objectives)
- [Data Description](#Data_Description)
- [Data Structure & Checks](#Data_Structure_&_Checks)
- [Executive Summary](#Executive_Summary)
- [Insights Deep Dive](#Insights_Deep_Dive)
  - [Energy Consumption](#Energy_Consumption)
  - [Smartmeter](#Smartmeter)
  - [Self Production](#Self_Production)
- [Recommendations](#Recommendations)
- [Assumptions and Caveats](#Assumptions_and_Caveats)

## Objectives
Energy Consumption Analysis: To assess patterns related to energy consumption and key factors that affect them
Smartmeter Analysis:  To investigate trends relate smart meter adoption
Self-Production Analysis: To analyse city and country wide trends that relate renewable energy and self reliance

## Data Description
The analyst is based on a rich dataset encompassing several key aspects to the Dutch energy system.
1. Geographical Details: Geographical data that details the regions where the providers operate at a regional, zip, city and street level. This information can be used to evaluate and execute stratigies down to the regional level.

2. Connection Details: The information provides details for connections in terms of where they are located, if they’re active, how many there are, and the type of connection. Information such as the following allow for determine trends in connection growth and how they impact consumption levels and efficiency.

3. Consumption Details: The datasets provide information related to the amount energy consumed overall, how much was given back to the grid and when they were consumed. Consumption details make it possible to understand patterns related to energy consumption the key factors that affect them and how to further improve rewenable energy consumption.

The use of geographical, connection and consumption details allow for a deeper understanding about the production of Dutch energy, and in turn the action required to increase sustainable energy use. By focusing on key factors and their effects, effective steps can be undertaken. 

The SQL queries used to inspect and clean the data for this analysis can be found here

DAX measures used in power query can be found [here](assets/DAX/)

## Data Structure & Checks
Excel Power Pivot was used to combine 8 million records from 150 files from kaggle and separate them into 2 different datasets, one for electricity and one for gas. A description for both [unedited](assets/ERD/Unedited) and [edited](assets/ERD/Edited/ERDDutch.png) data structure is as follows:

## Executive Summary

The data suggests that the oligopoly of Stedin, Liander and Enexis made up 97% of energy consumption in the country and 91% of gas consumption. Stedin is based in the regions of Rotterdam, Arnhem and Amsterdam. Liander throughout the idle of the country and Enexis in both south and northern outskirts. All other companies have niche markets that they supply to, E.g Endurise in the South-west on the France border. 

Over the past eight years, total electricity consumption in the Netherlands has remained relatively stable, though per-connection usage has declined due to increased energy efficiency and widespread adoption of LED lighting. While smart meter adoption for electricity has grown significantly, reaching 72% by 2020, full adoption is expected to take several more decades. Gas consumption, on the other hand, has seen a steady decline, despite the number of connections increasing. This reduction is largely driven by improvements in energy efficiency, increased use of renewable energy sources like solar power and heat pumps, and existing government incentives. Unlike electricity, where the highest consumption per household is concentrated in specific regions, gas usage remains more evenly spread across major cities.

Regional differences in energy production and self-sufficiency are notable, with Enexis outperforming other providers due to its presence in the northeast, where there is more space for wind and solar energy generation. In contrast, Stedin lags in self-production as its cities are located in densely populated areas with limited space for renewable infrastructure. The strong correlation between smart meter adoption and low-tariff electricity consumption, particularly in Liander cities, highlights shifting consumer behaviors. However, gas consumption does not follow this trend due to differences in pricing structures. Urbanization also plays a role in limiting self-production capabilities, as densely packed high-rise buildings have fewer opportunities for solar panel installations compared to rural areas.

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
Continue to promote energy efficiency programs
Improve grid infrastructure
Continue to push smartmeter use especially in the Coteq and Endinet regions
Expand renewable energy in rural areas to potential handle more cities such as the ones in Stedin
Faclitate ways to improve energy efficieny and self production in high-energy areas

Focus on connections such as 1x25 for electricity and g6 for gas.

## Recommendations
1. Continue to promote energy efficiency programs and appliances such as LED lighting and heating-efficiency programs especially in the Stedin region of central Netherlands as they have the highest delivery percentage.

2. Improve grid infrastructure to better manage fluctuations in energy demand and supply, ensuring efficient distribution across regions.

3. Increase incentives and awareness campaigns to encourage households to adopt smart meters, reducing resistance to adoption. Furthermore, Provide real-time consumption insights and usage alerts through smart meter apps to help users optimize energy use. This should be focused in for Coteq and Endinet customers due to relatively low smart meter adoption.

4.  Facilitate policies that enable small-scale energy producers, such as households and businesses, to feed excess power back into the grid.

5. Explore solutions for high-density areas, such as shared solar installations on apartment buildings and community energy projects.

Lastly, customers with 1x25 connections also show low adoption.

## Assumptions and Caveats:
The province of Zeeland seems to be missing entirely, but this could be due to there being a fourth provider
Something is wrong with the historical (pre-2017) data for Eindhoven
Some cities seem to have multiple providers. This might actually be true, but seems unlikely for some larger cities in Enexis territory like Weert and Deventer
Some cities seem to be producing gas, this seems unlikely
There are many minor errors, such as 's Gravenhage appearing more than once (but overall I ignore this since there is one 's Gravenhage that is the right size, the others are almost negligibly small.
