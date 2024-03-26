# Chemical comp of ceramic clustering

## Overview
The energy dispersive X-ray fluorescence (EDXRF) was used to determine the chemical composition of celadon body and glaze in Longquan kiln (at Dayao County) and Jingdezhen kiln. Forty typical shards in four cultural eras were selected to investigate the raw materials and firing technology.

The aim is to deduce any groupings of glazings and body compositions to see if they were used over multiple eras or if certain techniques of production where era specific. 

## Methodology 
1. Null and negative values where removed as you cannot have a negative PPM of a sample.
2. The number of Glazed and Body samples where double checked to make sure we have a comparison to each cluster to see where these era's may overlap.
3. Asses the outliers in the data and high correlation factors that may cause multicollinearity, in which case PCA may need to be used and outliers removed.
4. Create a pipline that runs on the glazed and body data the uses bootstrapping (due to the fact there is a limited amount of data) and changes outliers to only 2 std's away. This is because only ~3% of values are outliers. We also use PCA to remove multicollinearity.
5. Use the elbow method to deduce the optimal number of groupings.
6. Create clusters using the optimal number of groupings and see if there are overlaps in the body and glaze clusters to understand if there where similar methods used at different times
7. Finally, deduce the key factors that decide the type of cluster by looking at the factor loadings on the PCA.

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
