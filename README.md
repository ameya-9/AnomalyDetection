# AnomalyDetection
## Introduction
This was a personal project to learn more about concepts like Anomaly detection, Feature Engineering and Information Visualisation.

## Details:
Dataset: Ambient temperature [dataset](https://github.com/numenta/NAB/blob/master/data/realKnownCause/ambient_temperature_system_failure.csv).
Python Libraries: Pandas, NumPy, Matplotlib.pyplot, Scipy and Math

## Methodology:
1. Did exploratory analysis to understand the data and more details since I was not sure what were the temperature values of ? 
2. Visualized the data to see existence of an underlying pattern.
3. Feature Engineering: Created new data values from the TimeStamp --> DayOfWeek, Month, Year, Hour, DayOfMonths, 
      - replaced NaNs by mean of the value depending upon the context
4. Detecting underlying patterns: Analyzed the data to seek if there is weekly, monthly or yearly patterns 
5. Visualizing the patterns and Statistics: Used Matplotlib to visualize the findings, showcase the statistics and finally the distribution of Temperature.
6. **Anomaly Detection- Statistical Model** after visualizing and seeing the normal distribution with outliers, to see monthly trend. Used 95% confidence interval to show outlier values below and above the interval ( with 3 Zscore or +/- 3 standard deviation from the mean)
## Findings:
    1. The temperature on Mondays and Sundays are outlier.
    2. Most anamolies were either early morning or late nigh suggesting, this has ot be a working space.
    3. August 2nd, November 4th, December 5th and May 12th were outliers.
    4. We see there is dipped temperature April/May.
 
 
November temperature vs Days (and outliers in red)
![November temp and outliers in red] (https://github.com/ameya-9/AnomalyDetection/blob/main/img/Nov-outlier.png)
