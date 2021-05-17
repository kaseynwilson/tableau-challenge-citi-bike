# Citi Bike Analysis 

### For this project I utilized the following datasets from https://www.citibikenyc.com/system-data
  * Jersey City 2019 files (January through December)
  * Jersey City 2020 files (January through December)

### This dataset includes: 

  * Trip Duration (seconds)
  * Start Time and Date
  * Stop Time and Date
  * Start Station Name
  * End Station Name
  * Station ID
  * Station Lat/Long
  * Bike ID
  * User Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
  * Gender (Zero=unknown; 1=male; 2=female)
  * Year of Birth

## Data Cleansing:
Using Jupyter Notebook I imported the 24 CSV files for the 2019 and 2020 datasets. I performed the following tasks in order to perform the desired analysis:
  * Concatenated the individual dataframes from the CSV files to ultimately have one dataframe
  * Updated gender values from 0-2 to descriptive string values of Unknown, Male and Female respectively.
  * Split the 'starttime' column into Date and Time field and further split the Date into Year, Month and Day in order to have Year and Month values for analysis. 
  * Dropped columns that were not needed for analysis
  * Used the Birth Year and newly created Year column to calculate the approximate age of the users. 
  * Renamed Columns to have uniform and descriptive column headers
  * Exported newly combined and cleansed dataframe to a CSV 

## Analysis and Conclusions:
  * The most popular stations are in downtown Jersey City. The train station is at Grove Street, leading this to be the most popular station by far. Light rail stations are also some of the most popular stations. 
  * Subscriber activity was down from 2019 to 2020, while customer activity increased during the same timeframe. With COVID-19 many workers began working from home in 2020 leading to reduced subscribers. Customer (non-subscription based) activity likely increased due to increased outdoor leisurely activity and exercise sought during COVID-19 and social distancing requirements.
  * Overall number of trips taken was down from 2019 to 2020. Most months show a significant decrease in the number of rides taken by men from 2019 to 2020. There was less of a change for women although there was still a decrease most months. More women shifted from subscription based to non-subscription based usage from 2019 to 2020. These changes  could be due to less women holding corporate jobs in downtown Jersey City or more women participating is bike riding for leisure/exercise.
  * There was an increase in the average duration of trips, while the number of trips actually decreased from 2019 to 2020. This further demonstrates the shift in bicycle usage from commute to leisure and exercise.
  * Younger riders (age 25 and below) tend to have longer average ride times. Younger riders would likely be riding for leisure vs. commute. 
Riders of retirement age also saw an increase in average ride time even with some outliers removed. Age may be falsified on some of these riders. This could also be due to use of bikes for leisure vs. commute as well. 
  * Outside of the outliers of age 50 and 51 there is more frequent usage with riders between mid-twenties to mid-thirties. 
  * With 2019 and 2020 combined Sunday saw the least amount of rides, while Monday-Saturday had similar levels of riders. 
  * Saturday and Sunday saw an increase in the number of riders from 2019 to 2020, while weekdays saw a decrease in ridership. With COVID-19 fewer people were working in the office leading to decreases in commute use of bikes. Weekend increases in usage can be attributed to increases in outdoor leisure and exercise seen due to social distancing requirements.

## Next Steps
  * Based on these findings there is a significant opportunity to increase ridership for leisure and exercise. Many companies are planning to keep work from home options in place or hybrid in office and work from home stances. Due to this we will likely see a continuation of fewer people utilizing bikes for commute purposes. 
  * Marketing efforts towards women seem to be effective with less loss in overall ridership with women. Targeting mean for increases in bike utilization for recreational purposes could help make up for reductions in commute usage. 
  * Organized bike rides that start at designated stations could help increase ridership. 
  * Marketing to younger riders that are high school and college age could help increase ridership as well. These users tend to ride for longer periods of time. This seems to be a relatively untapped market as there are relatively few riders. 
