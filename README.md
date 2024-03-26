# Chemical comp of ceramic clustering

## Overview
The energy dispersive X-ray fluorescence (EDXRF) was used to determine the chemical composition of celadon body and glaze in Longquan kiln (at Dayao County) and Jingdezhen kiln. Forty typical shards in four cultural eras were selected to investigate the raw materials and firing technology.

The aim is to deduce any groupings of glazings and body compositions to see if they were used over multiple eras or is certain techniques of production where era specific  

## Methodology 
1. Each metric was brought togethor at a month on month level from the .gov csv's.
2. Correlations were checked to see if their were any strongly correlating groups that later on could be disgarded. Gas transfers were dropped.
3. To see if there was any lag in the data the correlations of each lagged variable with transfers were displayed to see if any could be used to create a higher    quality coefficient.
4. The greatest lagged correlations where then added to the original data frame.
5. The correlation and Rsquared values were then calcualated for each metric to understand the strongest descriptive factors of customer switching and how much of   the variance each explained.
6. The coefficient produced by the strongest factors are then used to determine the number of monthly customer swtiches based on these.

##Results 
For data from the 06/23 and before the best **Customer Elasticity coefficients** are shown below:

| Metric                  | Customer Elasticity coefficient |
|-------------------------|---------------------------------|
| Liquid fuels            |     3100                        |
| Gas                     |     2614                        |
| inflation index 23 days | -7388000                        |
| Solid fuels 39 days     | -1754000                        |

## .gov file locations
- [Pay (£)](https://www.ons.gov.uk/employmentandlabourmarket/peopleinwork/earningsandworkinghours)
- [Energy Prices](https://www.gov.uk/government/statistical-data-sets/monthly-domestic-energy-price-stastics)
- [Inflation](https://www.ons.gov.uk/economy/inflationandpriceindices)
- [Customer switching](https://www.gov.uk/government/statistical-data-sets/quarterly-domestic-energy-switching-statistics)
- [Inflation](https://www.ons.gov.uk/economy/inflationandpriceindices)
