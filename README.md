# VBA_Challenge
## Overview of Project
This analysis examines volume and price information for 12 green energy stocks. The intention of this analysis is to discover which green stocks perform well, returning positive return on investment; and those that perform poorly, returning negative returns on investment. 

### Results
After analyzing Total Daily Volume, Starting Price and Ending Price for 2017, it appears that green stocks were performing very well as a whole. Of the 11 stocks analyzed, only one, TERP, has negative returns on investment, or lost investors from the start to the end of the year. In particular, DQ, SEDG, ENPH, and FSLR all had a rate of return over 100%, meaning the value of their shares more than doubled over 2017. 

![stocks_2017](https://github.com/BKroos/VBA_Challenge/blob/main/resources/stocks_2017.png)

However, once the analysis is run for 2018, the story dramatically shifts. Of those with more than doubled value, all but one saw their stock values fall over the course of 2018. In particular, DQ lost over half of its value. The only stock to maintain its growth from 2017 to end of year 2018 was ENPH, which saw a return of nearly 82%. This stock also traded at the highest volumes, suggesting perhaps a level of reliability in the value of the stock, but also perhaps an example of the survivorship bias, as the second highest volume recorded was the only other green stock to gain value in 2018, RUN. 

![stocks_2018](https://raw.githubusercontent.com/BKroos/VBA_Challenge/main/resources/stocks_2018.png)

One other result of this analysis was the need to refactor code. Originally, I wrote the VBA code in distinct conditionals, however this slowed the analysis and ate up unnecessary resources. To correct this, I instead refactored the code to its current state, utilizing nested for loops. As a result, the run-time quickened as can be seen in the screenshots below:

![VBA_Challenge_2017](https://raw.githubusercontent.com/BKroos/VBA_Challenge/main/resources/VBA_Challenge_2017.png)

![VBA_Challenge_2018](https://github.com/BKroos/VBA_Challenge/blob/main/resources/VBA_Challenge_2018.png)

### Summary
The advantages to refactoring code are obvious, by making your code lighter and quicker, you're conserving computer resources and yours and whoever is utilizing your analysis' time. However, the cons to refactoring is the risk that you break what was working in the first place, or chase a possible solution down the rabbit hole that leads nowhere, wasting your own time. 

These pros and cons were obvious in the VBA script, as I found refactoring to be a frustrating lift, especially knowing how it was supposed to work and continually needing to debug to get it back to that point. In the end, the marginal reduction in time and resources did not feel like a strong enough payoff for me to endorse the refactoring in this case. 
