# Surfs Up - Hawaii Weather Analysis Using SQLite

## Overview of Project

### Purpose

Our objective is to analyze weather trends for the months of June and Decemeber in order to help determine the viability of opening a surf and ice cream business in Oahu.

### Resources
- Data: [hawaii.sqlite](hawaii.sqlite)
- Software: Python 3.7.9, sqlalchemy 1.3.20, Visual Studio Code 1.52.1, pandas 1.1.3, numpy 1.19.2


## Project Results

### Data Generated

- [june_precip.png](Resources/june_precip.png)
- [dec_precip.png](Resources/dec_precip.png)
- [june_temps.png](Resources/june_temps.png) (displayed below on the left)
- [dec_temps.png](Resources/dec_temps.png) (displayed below on the right)

<img src='Resources/june_temps.png'> <img src='Resources/dec_temps.png'>

### Results
- Three key differences between June's weather and December's weather:
  1. The measures of central tendency are closer than I expected.
      - Means only differ by 3.9°F
      - Medians ('50%' in tables above) only differ by 4°F
  2. The minimum recorded temperature in December is 9°F less than the minimum recorded temperature in June
  3. The maximum recorded temperature in December is only 2°F less than the maximum recorded temperature in June

## Summary

### Conclusion

From our results we see that the temperatures in the months of June and December are not far off from each other with average temperatures falling between 71-75°F. Noticeable trends were that in December 75% of all temperature records were above 69°F and June's lowest recorded temperature was 64°F. These sound like promising statistics in order to open a year-round surf and ice cream shop.

### Queries
###### Queries that are referenced in this section can be found in [additional_queries.ipynb](Resources/additional_queries.ipynb)

1. The first additional query would retrieve the precipitation data for June from `Measurement.prcp`. After executing it we would see that 59% of June records had precipitation and 75% of the days with precipitation recorded less than 0.24 inches of rain.
2. The second query would pull the same data, but for the month of December. After executing it we would see that 64% of December records had precipitation and 75% of the days with precipitation recorded less than 0.33 inches of rain.
 
### Next Steps

- A question we need to ask ourselves is, "Are June and December the best months to look at to represent peak warm weather and peak cold weather?" From the thrid query, the answer appears to be no. From our dataset, January (not December) has the lowest average temperature and the months of July, August, September, and October all have average temperatures higher than June. 

- Another variable we could research mor indepth is where on the island would our surf and ice cream shop thrive. Are there sides of the island that have more rain or better surfing waves? Can we use the latitudes and longitudes of the stations to determine the precipitation part of this question?