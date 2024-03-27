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
From this we can conclude that body cluster 2 and glaze cluster 2 have their own groups and come from the same era leading to the overlap.
Body cluster 1 has 2 types of glazes that is used from glaze cluster 3 and 1 so a similar Body composition was used across era's with the glaze changing 

Cluster: Body :1 , glaze:1 , Overlap_rate: 0.36 
Cluster: Body :1 , glaze:3 , Overlap_rate: 0.42 
Cluster: Body :1 , glaze:2 , Overlap_rate: 0.02 
Cluster: Body :2 , glaze:1 , Overlap_rate: 0.0 
Cluster: Body :2 , glaze:3 , Overlap_rate: 0.05 
Cluster: Body :2 , glaze:2 , Overlap_rate: 0.48 

## .gov file locations
- [Pay (£)](https://www.ons.gov.uk/employmentandlabourmarket/peopleinwork/earningsandworkinghours)
- [Energy Prices](https://www.gov.uk/government/statistical-data-sets/monthly-domestic-energy-price-stastics)
- [Inflation](https://www.ons.gov.uk/economy/inflationandpriceindices)
- [Customer switching](https://www.gov.uk/government/statistical-data-sets/quarterly-domestic-energy-switching-statistics)
- [Inflation](https://www.ons.gov.uk/economy/inflationandpriceindices)
